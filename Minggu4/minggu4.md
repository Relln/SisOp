# JOBSHEET-3

## PRAKTIKUM 3
### Percobaan 1
1. ![Alt text for screen readers](images/Percobaan-1-1.png)
2. ![Alt text for screen readers](images/Percobaan-1-2.png)
3. ![Alt text for screen readers](images/Percobaan-1-3.png)
-  ![Alt text for screen readers](images/Percobaan-1-3(2).png)
5. ![Alt text for screen readers](images/Percobaan-1-4.png)
   a.) Karena folder B tidak kosong tapi ada isinya
   b.) Karena folder B sudah berhasil dihapus pada perintah sebelumnya. Sistem tidak bisa menampilkan isi folder yang sudah tidak ada.
6. ![Alt text for screen readers](images/Percobaan-1-5.png)
   a.) Karena jalur tersebut salah secara struktur. Di Linux, folder user berada di bawah /home/. Jadi, /relln/C tidak akan ditemukan karena sistem mencarinya langsung di root (/), bukan di dalam folder home.

### Percobaan 2
1.![Alt text for screen readers](images/Percobaan-2-1.png)
2.![Alt text for screen readers](images/Percobaan-2-2.png)
3.![Alt text for screen readers](images/Percobaan-2-3.png)

### Percobaan 3
1.![Alt text for screen readers](images/Percobaan-3-1.png)
- ![Alt text for screen readers](images/Percobaan-3-1(2).png)

### Percobaan 4
1.![Alt text for screen readers](images/Percobaan-4-1.png)

### Percobaan 5
1.![Alt text for screen readers](images/Percobaan-5-1.png)
2.![Alt text for screen readers](images/Percobaan-5-2.png)
3.![Alt text for screen readers](images/Percobaan-5-3.png)

### Percobaan 6
1.![Alt text for screen readers](images/Percobaan-6-1.png)

## Latihan
### Soal
Cobalah urutan perintah berikut:
![Alt text for screen readers](images/Soal-Latihan-1.png)
![Alt text for screen readers](images/Soal-Latihan-2.png)
![Alt text for screen readers](images/Soal-Latihan-3.png)

### Jawaban
1. ![Alt text for screen readers](images/Latihan-1.png)
2. ![Alt text for screen readers](images/Latihan-2.png)
3. ![Alt text for screen readers](images/Latihan-3.png)
4. ![Alt text for screen readers](images/Latihan-4.png)
5 & 6. ![Alt text for screen readers](images/Latihan-5&6.png)
7 & 8. ![Alt text for screen readers](images/Latihan-7&8.png)
9. ![Alt text for screen readers](images/Latihan-9.png)
10 & 11. ![Alt text for screen readers](images/Latihan-10&11.png)
a.) sistem akan menolak dengan pesan error. Ini karena Linux tidak mengizinkan pembiatan hard link untuk file spesial (perangkat hardware) demi keamanan dan integritas sistem file.
12 & 13. ![Alt text for screen readers](images/Latihan-12&13.png)
14 & 15. ![Alt text for screen readers](images/Latihan-14&15.png)



### Kesimpulan 
Kesimpulan Praktikum Sistem Operasi
> Navigasi dan Struktur Hirarki File
Saya telah mempraktikkan penggunaan perintah dasar seperti cd, ls, pwd, dan cat untuk menjelajahi struktur direktori Linux. Hal ini membuktikan bahwa Linux memiliki pengorganisasian file yang terpusat, di mana setiap direktori memiliki fungsi spesifik (seperti /bin untuk eksekusi perintah user dan /etc untuk konfigurasi sistem).

> Pemahaman Pseudo-filesystem (/proc)
Praktikum ini menunjukkan bahwa tidak semua "file" di Linux tersimpan di harddisk. Direktori /proc adalah jendela ke dalam kernel yang bersifat sementara (volatile), memungkinkan pengguna melihat informasi perangkat keras seperti CPU (cpuinfo) dan memori (meminfo) secara real-time.

> Manajemen File dan Direktori
Kamu telah berhasil melakukan operasi manipulasi file dasar, termasuk:
- Pembuatan dan Penghapusan: Menggunakan mkdir dan rmdir.
- Duplikasi dan Perpindahan: Menggunakan cp dan mv untuk mengelola data di dalam direktori home.

> Konsep Link (Symbolic Link)
Salah satu poin penting adalah pemahaman tentang link. Kamu belajar bahwa symbolic link bertindak sebagai penunjuk (shortcut) ke file atau perangkat lain, seperti yang kamu lakukan pada perangkat tty. Kamu juga memahami batasan hard link yang tidak dapat diterapkan pada file perangkat atau antar sistem file yang berbeda.

> Interaksi dengan Perangkat Hardware
Dengan melakukan cp hello.txt terminal, kamu membuktikan filosofi Linux bahwa "Everything is a file". Mengirim data ke file perangkat terminal (/dev/tty1) secara otomatis akan menampilkan data tersebut ke layar fisik pengguna.
