# publisher_module9

**1. How much data your publisher program will send to the message broker in one
run?**

Dalam satu kali run, program publisher kamu akan mengirim 5 buah pesan ke message broker, masing-masing berupa objek UserCreatedEventMessage yang berisi dua field (user_id dan user_name). Jadi, total data yang dikirim adalah 5 pesan bertipe event.

**2. The url of: “amqp://guest:guest@localhost:5672” is the same as in the subscriber
program, what does it mean?**

URL "amqp://guest:guest@localhost:5672" menunjukkan bahwa publisher dan subscriber terhubung ke message broker yang sama, yaitu RabbitMQ yang berjalan secara lokal (localhost) di port 5672, dengan menggunakan kredensial default (guest sebagai username dan password). Ini berarti mereka berada di jaringan atau mesin yang sama dan bisa saling bertukar pesan.

**3. Running RabbitMQ**
![RabbitMQ](images/pic1.png)

**4. Console Subscriber**
![Subscriber](images/pic2.png)
Pada gambar di atas, publisher mengirimkan 5 event ke message broker subscriber yang diproses karena pada console, terlihat bahwa ada 5 event.
![Chart Publisher](images/pic3.png)

**5. Spike**
![pic7](images/pic7.png)
Dapat dilihat bahwa terjadi spike pada grafik ketika publisher dijalankan berkali-kali dengan intensitas yang berbeda ke message broker. Hal ini dinamakan sebagai lonjakan message rates .