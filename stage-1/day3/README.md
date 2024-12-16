# Task
## 1. Menurutmu apa itu Git ? 
- Git adalah sebuah alat atau sistem yang digunakan untuk mengelola dan melacak perubahan pada file, terutama dalam proyek pengembangan _software_. seperti sedang bekerja dalam sebuah tim untuk membuat dokumen atau program, dan setiap orang di tim mengedit bagian yang berbeda. Git membantu mencatat setiap perubahan yang dilakukan, siapa yang melakukannya, dan kapan itu dilakukan. Jadi, kalau ada kesalahan atau ingin kembali ke versi sebelumnya, bisa melakukannya dengan efisien.

## 2. Gambarkan menurut kalian flow dari cara kerja Git ini seperti apa ?
![workflow git drawio](https://github.com/user-attachments/assets/d7719ec0-6ff4-45ac-bd3d-a1ccbca78f19)

## 3. Buatlah Dokumentasi tentang Command yang ada di Git (boleh di tambahkan beberapa command yang mungkin belum kita pelajari pada saat pembahasan di kelas)
| Command git        | Description        |
| -------------|-------------| 
| **git init** |membuat repository|
| **git --version** |untuk mengecek _version_ git pada VM|
| **git add** |untuk menambah atau menandai setiap perubahan yang ada menuju tahap commit|
| **git status** |untuk melihat status perubahan terakhir|
| **git commit** |melakukan deskripsi atau _note_ apa saja yang diubah| 
| **git pull** |untuk men-_download_ repository yang _existing_ dari _database versioning control system_ ke local|
| **git clone** | Membuat salinan penuh dari repository, termasuk semua riwayat perubahan pada _database versioning control system_ milik sendiri maupun milik orang lain|
| **git restore**| memulihkan berkas dan direktori yang dihapus dari staging area atau _worktree_ Git |
| **git rm**| menghapus berkas repository git|
| **git branch**| merubah atau menambah branch pada direktori yang digunakan|
| **git config**| untuk melakukan konfigurasi pada git, _mostly_ lebih sering digunakan untuk peruntukan penambahan user.name dan user.email|
| **git remote**| untuk melakukan _remote controlling_ serta mengelola koneksi antara local dan _database versioning control system_ yang dituju|
| **git push** |untuk meng-_upload_ repository yang _existing_ dari local pada _database versioning control system_|
| **ssh-keygen**| untuk membuat openSSH dari local dan di patch pada _database versioning control system_ yang digunakan|
| **ssh -T**| untuk mengecek koneksi openSSH apakah sudah terkoneksi apa belum|

## 4. Study Case
- Ada 2 Developer yang sedang melakukan development aplikasi dari perusahaan A sebut saja Reyhan dan Teguh mereka kebetulan sedang mengerjakan suatu proyek yang sama, dan mereka sedang mengerjakan file yang sama `index.html`. Reyhan membuat perubahan pada file index.html dan melakukan commit: `git add index.html;
git commit -m "fix: Typo on Description"`.  Teguh kebetulan juga membuat perubahan pada index.html dan melakukan commit: `git add index.html ; git commit -m "feat: Header Adjustment"`. Kemudia disini ternyata Reyhan melakukan `push` ke repository. Teguh, yang belum melakukan push, mencoba untuk melakukan push ke repositori. Karena ternyata ada perubahan baru di remote yang belum dimiliki Teguh, Git menolak push Teguh dan memberi tahu bahwa ada konflik. Disini Teguh harus melakukan Fix Conflict tersebut agar perubahan yang di buat oleh Teguh dapat tersimpan ke dalam repositori app tersebut. lalu bagaimana cara menangani case yang dimiliki oleh Teguh?

### a. Reyhan 
![image](https://github.com/user-attachments/assets/6e4fb298-b011-46db-a598-25bef68a8efc)

![image](https://github.com/user-attachments/assets/003b9337-e4f5-4dac-a52a-44116b14af40)

![image](https://github.com/user-attachments/assets/092b039c-e42f-4cc3-bb6f-c8f5ee6f9a71)

![image](https://github.com/user-attachments/assets/d3b3dc4d-d328-46e3-8386-7544d6b2d9a1)

![image](https://github.com/user-attachments/assets/a41209cc-f09e-4c22-9a55-b0a162952822)

![image](https://github.com/user-attachments/assets/20c79370-ff2f-46a4-9cfc-8c8087d8cd1e)

### b. Teguh
![image](https://github.com/user-attachments/assets/47cc1f55-17a0-4481-878c-1623cee0f2f3)

![image](https://github.com/user-attachments/assets/5db81aa0-2208-4e5b-9d5f-4d9a6599913e)

![image](https://github.com/user-attachments/assets/86931637-20b9-42a3-9e35-d2539678f527)

![image](https://github.com/user-attachments/assets/ec2eb30c-58e1-456e-b7e4-59e53d726c0e)

![image](https://github.com/user-attachments/assets/e7a543b1-e16b-4c02-946e-8cbd816a9935)

![image](https://github.com/user-attachments/assets/6c56ddd7-44e9-4f0d-b4cd-6e88f192dbb3)



