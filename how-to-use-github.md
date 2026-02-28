## CASE 1 — Push Kode PERTAMA KALI ke GitHub

```bash
# masuk ke folder project
cd path/project

# init git
git init

# hubungkan ke repo GitHub
git remote add origin https://github.com/username/repo-name.git

# cek remote
git remote -v

# add semua file
git add .

# commit pertama
git commit -m "Initial commit"

# set branch utama
git branch -M main

# push 
git push -u origin main

# apabila ingin force push 
git push -u origin main --force
```

## CASE 2 — Clone Repository GitHub ke Lokal

```bash
# clone repo
git clone https://github.com/username/repo-name.git

# masuk ke folder repo
cd repo-name
```

## CASE 3 — Perbaiki / Tambah Kode LALU Push (Tanpa Fork, Sebagai Collaborator)

```bash
# buat branch baru
git checkout -b nama-branch

# cek status
git status

# edit kode (via editor)

# add perubahan
git add .

# commit perubahan
git commit -m "fix: perbaiki bug X"

# push branch
git push origin nama-branch
```

Lanjut **Create Pull Request** di GitHub

## CASE 4 Update Kode Lagi di Branch yang Sama

```bash
# pastikan di branch yang benar
git branch

# edit kode

# add & commit
git add .
git commit -m "chore: update logic"

# push ulang
git push
```

## CASE 5 — Ambil Update Terbaru dari GitHub

```bash
# pindah ke main
git checkout main

# ambil update
git pull origin main
```

## CASE 6 Batalkan Perubahan (Kalau Salah Edit)

```bash
# batalkan perubahan file
git restore nama-file

# batalkan semua perubahan
git restore .

# batalkan staging
git reset

# Hapus cache pada git apabila masih terdapat cache
git rm --cached NOTE.md
```

## CASE 7 Pindah & Kelola Branch

```bash
# lihat branch
git branch

# pindah branch
git checkout nama-branch

# hapus branch lokal
git branch -d nama-branch
```

## Cheat Sheet Paling Penting

```bash
git status
git branch
git remote -v
git log --oneline
```

