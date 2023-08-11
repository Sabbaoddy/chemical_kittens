# chemical_kittens
learning about telegram bot

Membuat Telegram bot dengan Bash tidaklah umum, karena sebagian besar bot Telegram dikembangkan menggunakan bahasa pemrograman lain seperti Python, Node.js, atau Java. Namun, Anda masih dapat menggunakan Bash untuk melakukan beberapa tugas sederhana, seperti mengirim pesan teks melalui API Telegram.

Sebagai contoh, berikut adalah contoh skrip Bash yang dapat Anda gunakan untuk mengirim pesan teks melalui bot Telegram menggunakan permintaan HTTP (HTTP request). Anda perlu mengganti `<YOUR_BOT_TOKEN>` dengan token bot Telegram Anda dan `<CHAT_ID>` dengan ID obrolan (chat) yang ingin Anda kirim pesan.

```bash
#!/bin/bash

BOT_TOKEN="<YOUR_BOT_TOKEN>"
CHAT_ID="<CHAT_ID>"
MESSAGE="Halo dari bot Telegram!"

API_URL="https://api.telegram.org/bot$BOT_TOKEN/sendMessage"

curl -s -X POST "$API_URL" -d "chat_id=$CHAT_ID" -d "text=$MESSAGE"
```

Pastikan Anda memiliki perintah `curl` yang terpasang di sistem Anda. Anda juga perlu mengaktifkan mode script dengan memberikan izin eksekusi ke skrip Anda (`chmod +x nama-skrip.sh`).

Namun, untuk pengembangan lebih lanjut dan penggunaan yang lebih kompleks, disarankan untuk menggunakan bahasa pemrograman yang lebih sesuai seperti Python atau JavaScript. Dalam bahasa-bahasa tersebut, tersedia pustaka-pustaka yang lebih nyaman untuk berinteraksi dengan API Telegram.

Untuk informasi lebih lanjut tentang cara membuat bot Telegram dengan bahasa pemrograman lain, silakan lihat dokumentasi resmi Telegram API dan dokumentasi bahasa pemrograman yang Anda pilih.
