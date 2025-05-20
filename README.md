# Halo GitHub!

Workflow Secara Sederhana
1. Buka repository di IDE. Kalau download dari github, bisa dengan clone (``` git clone <url-repository> ```)
2. Lakukan hal yang diinginkan (tambah/edit/hapus file)
3. Masukkan file ke staging area (``` git add . ```), lalu commit (``` git commit -m "<Pesan perubahan>" ```). Kalau mau langsung, bisa gunakan (``` git commit -am "<Pesan perubahan>" ```)
4. Push ke repository (``` git push origin <nama-branch> ```)

# Penjelasan

Berikut merupakan beberapa command penting untuk memahami workflow dasar github

---

Useful Command
1. ``` git status ``` = menampilkan status dari repository
2. ``` git branch ``` = menampilkan daftar branch
3. ``` git log ``` = menampilkan informasi commit yang telah dilakukan

---

Membuat Repository Baru
1. ``` git init ``` = membuat local repository
2. ``` git clone <url-repository> ``` = clone repository dari github

---

Menambahkan File ke Staging Area
1. ``` git add <nama-file> ``` = file ditambahkan ke staging area (tempat sementara sebelum file dicommit)
2. ``` git add . ``` = menambahkan semua file ke staging area

---

Commit Perubahan
1. ``` git commit -m "<Pesan perubahan>" ``` = perubahan yang ada akan disimpan, -m berfungsi sebagai pesan dari perubahan
2. ``` git commit -am "<Pesan perubahan>" ``` = apabila belum di add, -am akan sekaligus mengadd

---

Push ke Remote Repository
1. ``` git push origin <nama-branch> ``` = perubahan akan dipush ke dalam repository github

---

Membuat Branch
1. ``` git -b <nama-branch> ``` = membuat branch baru
2. ``` git checkout <nama-branch> ``` = pindah branch
3. ``` git checkout -b <nama-branch> ``` = membuat branch baru, sekaligus pindah

---

Log Commit
1. ``` git log -<Berapa jumlah commit terakhir> ``` = menampilkan informasi commit sebanyak yang diinginkan, dari yang terbaru
2. ``` git log <nama-file> ``` = menampilkan informasi commit file tertentu
3. ``` git log --since='Month Day Year' ``` = menampilkan informasi commit dari waktu yang diinginkan
4. ``` git log --until='Month Day Year' ``` = menampilkan informasi commit sampai waktu yang diinginkan
5. ``` git show <8-10 hash pertama> ``` = menampilkan detail dari commit (tags, trees, blobs)

---

Membandingkan Version File
1. ``` git diff <nama-file> ``` = menampilkan perbedaan antara version file yang terakhir di-commit dan version modified (belum di-add)
2. ``` git diff --staged <nama-file> ``` = menampilkan perbedaan antara version file yang terakhir di-commit dan version staging area
3. ``` git diff <8-10 hash pertama> <8-10 hash pertama> ``` = menampilkan perbedaan antara 2 file yang sudah di-commit
4. ``` git diff HEAD~1 HEAD ``` = menampilkan perbedaan antara 2 file terakhir yang sudah di-commit (HEAD = commit terakhir)

---

Reverting dan Restoring File
1. ``` git revert HEAD ``` = mengembalikan commit terakhir dan langsung mencommitnya (membuka text editor untuk memberikan message)
2. ``` git revert --no-edit HEAD ``` = mengembalikan tanpa membuka text editor dan langsung mencommitnya
3. ``` git revert -n HEAD ``` = mengembalikan tanpa mencommitnya (ada di stage area)
4. ``` git checkout HEAD~1 -- <nama-file> ``` = mengembalikan hanya satu file saja dari commit terkahir
5. ``` git restore --staged ``` = menghapus semua file dari staging area
6. ``` git restore --staged <nama-file> ``` = menghapus hanya satu file saja dari staging area