# portfolio-vito

<script src="https://cdnjs.cloudflare.com/ajax/libs/clipboard.js/2.0.6/clipboard.min.js"></script>
<button class="btn-clipboard" data-clipboard-target="#code-block">
    Copy Code
</button>
<script>
    new ClipboardJS('.btn-clipboard');
</script>

#Basic Git Commands

- Inisialisasi Repository Baru
  git init

- Menambahkan File ke Staging Area
  git add filename.txt
  Commit Perubahan

git commit -m "Pesan commit"
Melihat Status Repository

git status
Melihat Riwayat Commit

git log
Menghapus File dari Staging Area

git reset HEAD filename.txt
Menghapus File dari Repository

git rm filename.txt
Intermediate Git Commands
Membuat Branch Baru
git branch nama-branch
Berpindah ke Branch

git checkout nama-branch
Menggabungkan Branch

git merge nama-branch
Menampilkan Semua Branch

git branch
Menampilkan Semua Remote

git remote -v
Menambahkan Remote Repository

git remote add origin url-repository
Push Perubahan ke Remote Repository

git push origin nama-branch
Menarik Perubahan dari Remote Repository

git pull origin nama-branch
Advanced Git Commands
Menghapus Branch yang Sudah Digabung

git branch -d nama-branch
Menunjukkan Perbedaan antara Branch

bash
Salin kode
git diff nama-branch1..nama-branch2
Stashing Perubahan Sementara

git stash
git stash apply
Mengubah Commit Terakhir (Amend)

git commit --amend
Rebasing Branch

git rebase nama-branch
Menghapus Tag

git tag -d nama-tag
Menyaring Komit Menggunakan filter-branch

git filter-branch --env-filter 'if [ "$GIT_AUTHOR_EMAIL" = "old@example.com" ]; then export GIT_AUTHOR_EMAIL="new@example.com"; fi' -- --all
Membuat dan Mengelola Submodule

git submodule add url-repository path
git submodule update --init
Melakukan Rebase Interaktif

git rebase -i HEAD~n
Menelusuri Riwayat Perubahan File

git log -- filename.txt
