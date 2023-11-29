Saat ini saya mengalami masalah tentang partisi data saya terkena read-only filesystem :

langkah yang saya ambil menggunakan 

ntfsfix
langkah - langkah : 
1. melakukan check inisial partisi menggunakan perintah fdisk -l 
2. exsekusi perintah ntfsfix dengan sudo ntfsfix /dev/nvme0n1p3

hasil = Tidak ada Perubahan

Mematikan Fastboot di windows 
langkah-langkah
1. Reboot dan masuk ke windows
2. masuk ke control panel ->system and security -> power option -> masuk sebagai administrator
3. matikan opsi Fastboot

hasil = berhasil

conclusion = jangan lupa mematikan fastboot saat melakukan dualboot windows dan linux karena windows dapat mempengaruhi partisi agar
bisa booting lebih cepat dan dapat menyebabkan read-only filesystem saat dibuka di linux

