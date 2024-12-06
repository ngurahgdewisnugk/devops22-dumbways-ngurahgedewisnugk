# Task Day 1 -- Introduction To DevOps

## 1. Menurutmu apa itu DevOps (coba jelaskan dengan bahasa kamu sendiri)
- DevOps adalah cara kerja yang menggabungkan tim pengembang perangkat lunak (Developer) dan tim operasi teknologi (Operations) agar bisa bekerja sama dengan lebih baik. dengan bahasa sederhananya Tujuannya adalah membuat proses *building*, *testing*, dan *launching* aplikasi menjadi lebih cepat, efisien, dan andal.
DevOps memastikan mereka bekerja bersama, berbagi informasi, dan menggunakan alat yang membantu agar semua berjalan lancar. 
Karena DevOps bukan hanya tentang alat atau teknologi, tapi juga tentang budaya kerja yang mendukung kolaborasi dan peningkatan berkelanjutan.

## 2. Buatlah 1 Virtual Machine (bebas ingin menggunakan Multipass, VMware, Virtualbox, etc) dengan spec menyesuaikan.
#### Membuat 1 Virtual Machine menggunakan Multipass

- a.	install dulu multipass pada link ini https://multipass.run/install
  ![image](https://github.com/user-attachments/assets/982ede00-4b0c-4849-8a60-de0ef762fd6b)
- b.	Tentukan berdasarkan OS yang digunakan. 
![image](https://github.com/user-attachments/assets/f984e9e9-140c-4b87-a3c0-bf927e0e6bcc)
- c.	Setelah Terinstall, dia akan menampilkan berbagai image instace OS yang dapat digunakan, tentukan images yang ingin digunakan
![image](https://github.com/user-attachments/assets/989bfd3c-b68f-488d-b775-a242c9ffb020)
- d.	Sebelum Launch, pilih terlebih dahulu tombol setting berdasarkan images OS yang ingin dijalankan, **untuk melakukan konfigurasi dan menyesuaikan spec yang digunakan**
  ![image](https://github.com/user-attachments/assets/dcf4b804-4e82-47f3-a2d5-2383f107c80d)
  ![image](https://github.com/user-attachments/assets/6863f4e1-fb56-4965-b3bb-ebd0d768b0b8)
- e.	Setelah ditentukan spec yang dibutuhkan serta konfigurasi yang disesuaikan, lakukan launch
  ![image](https://github.com/user-attachments/assets/831f3601-b683-4723-8159-871eb78b530b)
- f.	Multipass pun membuat instace yang dibutuhkan
  ![image](https://github.com/user-attachments/assets/780a0b48-f5dc-4056-9154-3350ba40df87)
- g.	Instace pun terinstall
  ![image](https://github.com/user-attachments/assets/3de3e882-5848-4496-bcc2-bc25c28bc6ef)
- h.	Untuk pembuktian, silahkan coba ping ke google.com untuk pengetesan koneksi bridge network pada instace yang sudah dibuat.
  ![image](https://github.com/user-attachments/assets/5277a0e2-05bb-4329-a7eb-b52da6c96431)

## 3. Install apache2 WebServer ke dalam Virtual Machine yang telah kalian buat.
- a.	pertama lakukan upgrade dan update version terlebih dahulu, agar system *up-to-date*
  
   `
  sudo apt upgrade; sudo apt update
   `
  
  ![image](https://github.com/user-attachments/assets/1b4e6dde-03e8-43f3-bdcb-4f7e56cfd833)
- b.	setelah itu lakukan install apache2 web server

  `
  sudo apt install apache2
  `
  
  ![image](https://github.com/user-attachments/assets/6ce1ff56-b2cd-4f61-9b70-119c0498f36c)
- c.	setelah terinstall apache2 web server lakukan pengecekan service apache2
  `
  systemctl status apache2
  `
  
  ![image](https://github.com/user-attachments/assets/1b052c07-3726-4916-9277-e718339fee94)
- d. jika statusnya sudah ***running***, silahkan lakukan pengecekan di web browser local menggunakan ***ip address*** dari server
  ![image](https://github.com/user-attachments/assets/8ee1a9a1-7ba0-4f5a-a46b-781fa39fc9dc)

> [!NOTE]
> Untuk Windows pastikan tambah ip address server kalian pada file **hosts** yang terletak di *C:\Windows\System32\drivers\etc*, sesuai ip address yang digunakan pada server



