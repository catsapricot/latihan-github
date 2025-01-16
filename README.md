# Halo GitHub!

Berikut merupakan beberapa command penting untuk memahami workflow dasar github

---

Useful Command
1. ``` git status ``` = menampilkan status dari repository
2. ``` git branch ``` = menampilkan daftar branch

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