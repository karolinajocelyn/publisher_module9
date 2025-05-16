# publisher_module9

1. How much data your publisher program will send to the message broker in one
run?

Dalam satu kali run, program publisher kamu akan mengirim 5 buah pesan ke message broker, masing-masing berupa objek UserCreatedEventMessage yang berisi dua field (user_id dan user_name). Jadi, total data yang dikirim adalah 5 pesan bertipe event.

2. The url of: “amqp://guest:guest@localhost:5672” is the same as in the subscriber
program, what does it mean?

URL "amqp://guest:guest@localhost:5672" menunjukkan bahwa publisher dan subscriber terhubung ke message broker yang sama, yaitu RabbitMQ yang berjalan secara lokal (localhost) di port 5672, dengan menggunakan kredensial default (guest sebagai username dan password). Ini berarti mereka berada di jaringan atau mesin yang sama dan bisa saling bertukar pesan.
