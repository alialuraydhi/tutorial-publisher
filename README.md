a. Berapa banyak data yang dikirimkan oleh program publisher ke message broker dalam satu kali jalan?
Program publisher akan mengirimkan sebanyak 5 pesan (event) ke message broker dalam satu kali eksekusi. Setiap pesan tersebut merepresentasikan event user_created.
Setiap pesan berisi data dengan tipe UserCreatedEventMessage yang memiliki dua properti utama:

user_id: Merupakan string yang berisi ID pengguna (dalam bentuk angka).

user_name: Merupakan string nama pengguna, diawali dengan NPM saya. Contohnya: "2306275992-Amir".

b. URL `amqp://guest:guest@localhost:5672` juga digunakan dalam program subscriber. Apa artinya?
Hal ini berarti bahwa publisher dan subscriber terhubung ke broker pesan yang sama, yaitu yang berada di alamat `amqp://guest:guest@localhost:5672`.
Publisher berfungsi untuk mengirimkan pesan ke broker, sedangkan subscriber berperan untuk menerima pesan dari broker tersebut. Dengan menggunakan URL yang sama, keduanya bisa berinteraksi dalam satu sistem pengiriman pesan yang terintegrasi.


Running RabbitMQ

![image](https://github.com/user-attachments/assets/254a039e-755b-42af-bef4-13245908a307)

