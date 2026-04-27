# JOBSHEET - 9

## LATIHAN
### Latihan 9.1
Modifikasi laporan-sistem.sh agar menyimpan output ke file laporan-YYYY-MM-DD.txt sekaligus menampilkannya di terminal. Petunjuk:
gunakan tee yang sudah dipelajari di bab sebelumnya.
= <img width="1053" height="460" alt="image" src="https://github.com/user-attachments/assets/eaaac886-9f79-49e6-8146-c94cb5a4b00b" />
<img width="954" height="658" alt="image" src="https://github.com/user-attachments/assets/8edb5d8b-c2f2-47b1-b167-9d8b4b5cf0ef" />

### Latihan 9.2
Buat script kalkulator.sh yang menerima tiga argumen: <angka1>
<operator> <angka2> dengan operator +, -, *, atau /. Contoh:
./kalkulator.sh 20 + 5 menghasilkan 25. Gunakan case untuk memilih
operasi, dan validasi jika argumen tidak lengkap.
<img width="810" height="766" alt="image" src="https://github.com/user-attachments/assets/d4c966ac-36e9-4982-b100-b927630ccd36" />
<img width="894" height="345" alt="image" src="https://github.com/user-attachments/assets/c51c88d1-ac8d-4c05-a208-912e29306e82" />
<img width="644" height="60" alt="image" src="https://github.com/user-attachments/assets/5f332921-0b7e-4bed-832a-6d7a707fa8a0" />

### Latihan 9.3
Tambahkan ke script grading-batch.sh sebuah ringkasan di bagian bawah yang menampilkan: jumlah mahasiswa per grade (A, B, C, D, E) menggunakan
perulangan for kedua yang mengiterasi array MAHASISWA
<img width="966" height="771" alt="image" src="https://github.com/user-attachments/assets/f00e161e-468c-4fee-bb65-27cc1f384298" />
<img width="554" height="428" alt="image" src="https://github.com/user-attachments/assets/33dfbf52-454a-47dd-9fde-02bb53165d35" />


### Latihan 9.4
Tambahkan fungsi konfirmasi() ke lib-validasi.sh. Fungsi ini menampilkan pertanyaan, membaca input Y/N dari user, mengembalikan
0 jika Y dan 1 jika N. Buat script demo yang memanggil fungsi ini sebelum menghapus sebuah file.
Terakhir, kita masuk ke Latihan 9.4. Di sini kita akan belajar membuat Library Script (file yang berisi kumpulan fungsi) dan cara memanggil fungsi tersebut dari script lain.
<img width="701" height="513" alt="image" src="https://github.com/user-attachments/assets/44ac5fe3-e47c-42bb-ba49-5e509fceab1a" />
<img width="875" height="456" alt="image" src="https://github.com/user-attachments/assets/60778b0d-aba1-45a8-94e0-627e690770ce" />
<img width="704" height="115" alt="image" src="https://github.com/user-attachments/assets/2865a282-d841-4864-b0fe-eff62298fda2" />

### Latihan 9.5
Script debug-latihan.sh tidak menangani direktori yang tidak ada. Perbaiki
dengan menambahkan:
• set -e di baris kedua
• Pengecekan -d "$DIREKTORI" sebelum memanggil du
• Pesan error yang informatif jika direktori tidak ditemukan
Uji dengan direktori yang tidak ada.
<img width="962" height="652" alt="image" src="https://github.com/user-attachments/assets/17f662bc-35d7-4cfd-8ea9-d30138898fe8" />
<img width="959" height="91" alt="image" src="https://github.com/user-attachments/assets/984ab667-a39f-4a08-8b63-ec9b113c6448" />
<img width="588" height="90" alt="image" src="https://github.com/user-attachments/assets/6c5bb200-6e7a-4de1-bf35-531cf9d533a0" />


## PRAKTIKUM
### Tugas 1 Script Absensi Kelas
Konteks: instruktur mencatat kehadiran mahasiswa dari command line.
1. Buat script absensi.sh yang:
• Menerima argumen nama mahasiswa dan status (hadir/izin/alpha)
• Menyimpan entri ke absensi-YYYY-MM-DD.txt dengan format [HH:MM]
NAMA - STATUS
• Opsi -r: tampilkan rekapitulasi (jumlah per status)
• Opsi -h: tampilkan bantuan
2. Rekam minimal 5 entri dan tampilkan rekapitulasinya.
Konsep wajib: variabel, parameter posisional, getopts, if, for, fungsi, dan
redirection ke file.
<img width="827" height="713" alt="image" src="https://github.com/user-attachments/assets/136ea4cd-2540-4ca3-b49a-57263185a1d0" />
<img width="865" height="544" alt="image" src="https://github.com/user-attachments/assets/a21ee5e1-64c3-4b9b-81e1-ef67f5a2baee" />
<img width="709" height="280" alt="image" src="https://github.com/user-attachments/assets/1611ff98-7732-48cb-a299-504bfb42c240" />
<img width="602" height="139" alt="image" src="https://github.com/user-attachments/assets/5e3976b0-76c3-4fcb-9302-8339eb603076" />

### Tugas 2 Script Health Check Sistem
Konteks: administrator membuat pemeriksaan kondisi server sebelum maintenance.
1. Buat script healthcheck.sh menggunakan template profesional dari bagian
Best Practices.
2. Script menampilkan: tanggal/waktu, hostname, uptime, penggunaan CPU,
memori, dan disk untuk setiap filesystem yang terpasang.
3. Jika penggunaan disk mana pun melebihi 80%, tampilkan peringatan.
4. Simpan hasil ke healthcheck-YYYY-MM-DD.log dan tampilkan ke terminal
sekaligus menggunakan tee.
5. Opsi -t <persen> mengubah batas peringatan disk (default 80).
Konsep wajib: set -euo pipefail, trap, getopts, fungsi dengan local,
for, if, dan tee.
<img width="834" height="711" alt="image" src="https://github.com/user-attachments/assets/d6fcd1a8-d942-4fe5-9b78-b4dfeb90f34c" />
<img width="952" height="765" alt="image" src="https://github.com/user-attachments/assets/d4f85245-1520-4147-b558-5f9dd0cd0bda" />
<img width="923" height="745" alt="image" src="https://github.com/user-attachments/assets/efc2efca-ea0a-4a2e-b33a-c3ec02b5cd79" />
<img width="831" height="713" alt="image" src="https://github.com/user-attachments/assets/92b753a1-d2e2-4549-8895-0ba67d41295a" />
<img width="955" height="747" alt="image" src="https://github.com/user-attachments/assets/d8d5d25c-0f49-40e6-bcca-2f2c11bcb223" />
<img width="830" height="648" alt="image" src="https://github.com/user-attachments/assets/af3aa2ac-ca74-453b-b741-ac663d54f858" />





