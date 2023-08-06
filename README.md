# linuxcommand
important command line in linux:
* `systemctl daemon-reload` untuk mengaktifkan _service_ yang baru di unggah
* `systemctl [start|stop] [name.service]` untuk menghidupkan dan mematikan _service_
* `systemctl [enable|disable] [name.service]` untuk menghidupkan dan mematikan _service_ setiap kali _reboot_
* `systemctl list-units --type=service --state=running` untuk melihat server mana saja yang aktif.
* `netstat -tulpen |grep 80` ini perintah tambahan untuk melihat webserver mana saja yang sedang aktif.

changing nginx configuration:\
Setelah melakukan perubahan configurasi pada sites-available kita harus hapus sites-enable dengan code
* `rm /etc/nginx/sites-enabled/server.conf`\
lalu jalankan code berikut ini
* `ln -s /etc/nginx/sites-available/server.conf /etc/nginx/sites-enabled/server.conf`
