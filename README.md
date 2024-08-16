# portfolio-vito

# Basic Git Commands

<h3>Inisialisasi Repository Baru</h3>
<pre>
  <code id="init-repo">
    git init
  </code>
</pre>
<button onclick="copyCode('init-repo')">Copy</button>

<h3>Menambahkan File ke Staging Area</h3>
<pre>
  <code id="add-file">
    git add filename.txt
  </code>
</pre>
<button onclick="copyCode('add-file')">Copy</button>

<h3>Commit Perubahan</h3>
<pre>
  <code id="commit">
    git commit -m "Pesan commit"
  </code>
</pre>
<button onclick="copyCode('commit')">Copy</button>

<h3>Melihat Status Repository</h3>
<pre>
  <code id="status">
    git status
  </code>
</pre>
<button onclick="copyCode('status')">Copy</button>

<h3>Melihat Riwayat Commit</h3>
<pre>
  <code id="log">
    git log
  </code>
</pre>
<button onclick="copyCode('log')">Copy</button>

<h3>Menghapus File dari Staging Area</h3>
<pre>
  <code id="reset">
    git reset HEAD filename.txt
  </code>
</pre>
<button onclick="copyCode('reset')">Copy</button>

<h3>Menghapus File dari Repository</h3>
<pre>
  <code id="rm">
    git rm filename.txt
  </code>
</pre>
<button onclick="copyCode('rm')">Copy</button>

# Intermediate Git Commands

<h3>Membuat Branch Baru</h3>
<pre>
  <code id="branch-create">
    git branch nama-branch
  </code>
</pre>
<button onclick="copyCode('branch-create')">Copy</button>

<h3>Berpindah ke Branch</h3>
<pre>
  <code id="branch-checkout">
    git checkout nama-branch
  </code>
</pre>
<button onclick="copyCode('branch-checkout')">Copy</button>

<h3>Menggabungkan Branch</h3>
<pre>
  <code id="merge">
    git merge nama-branch
  </code>
</pre>
<button onclick="copyCode('merge')">Copy</button>

<h3>Menampilkan Semua Branch</h3>
<pre>
  <code id="branch-list">
    git branch
  </code>
</pre>
<button onclick="copyCode('branch-list')">Copy</button>

<h3>Menampilkan Semua Remote</h3>
<pre>
  <code id="remote-list">
    git remote -v
  </code>
</pre>
<button onclick="copyCode('remote-list')">Copy</button>

<h3>Menambahkan Remote Repository</h3>
<pre>
  <code id="remote-add">
    git remote add origin url-repository
  </code>
</pre>
<button onclick="copyCode('remote-add')">Copy</button>

<h3>Push Perubahan ke Remote Repository</h3>
<pre>
  <code id="push">
    git push origin nama-branch
  </code>
</pre>
<button onclick="copyCode('push')">Copy</button>

<h3>Menarik Perubahan dari Remote Repository</h3>
<pre>
  <code id="pull">
    git pull origin nama-branch
  </code>
</pre>
<button onclick="copyCode('pull')">Copy</button>

# Advanced Git Commands

<h3>Menghapus Branch yang Sudah Digabung</h3>
<pre>
  <code id="branch-delete">
    git branch -d nama-branch
  </code>
</pre>
<button onclick="copyCode('branch-delete')">Copy</button>

<h3>Menunjukkan Perbedaan antara Branch</h3>
<pre>
  <code id="diff">
    git diff nama-branch1..nama-branch2
  </code>
</pre>
<button onclick="copyCode('diff')">Copy</button>

<h3>Stashing Perubahan Sementara</h3>
<pre>
  <code id="stash">
    git stash
    git stash apply
  </code>
</pre>
<button onclick="copyCode('stash')">Copy</button>

<h3>Mengubah Commit Terakhir (Amend)</h3>
<pre>
  <code id="amend">
    git commit --amend
  </code>
</pre>
<button onclick="copyCode('amend')">Copy</button>

<h3>Rebasing Branch</h3>
<pre>
  <code id="rebase">
    git rebase nama-branch
  </code>
</pre>
<button onclick="copyCode('rebase')">Copy</button>

<h3>Menghapus Tag</h3>
<pre>
  <code id="tag-delete">
    git tag -d nama-tag
  </code>
</pre>
<button onclick="copyCode('tag-delete')">Copy</button>

<h3>Menyaring Komit Menggunakan filter-branch</h3>
<pre>
  <code id="filter-branch">
    git filter-branch --env-filter 'if [ "$GIT_AUTHOR_EMAIL" = "old@example.com" ]; then export GIT_AUTHOR_EMAIL="new@example.com"; fi' -- --all
  </code>
</pre>
<button onclick="copyCode('filter-branch')">Copy</button>

<h3>Membuat dan Mengelola Submodule</h3>
<pre>
  <code id="submodule">
    git submodule add url-repository path
    git submodule update --init
  </code>
</pre>
<button onclick="copyCode('submodule')">Copy</button>

<h3>Melakukan Rebase Interaktif</h3>
<pre>
  <code id="rebase-interactive">
    git rebase -i HEAD~n
  </code>
</pre>
<button onclick="copyCode('rebase-interactive')">Copy</button>

<h3>Menelusuri Riwayat Perubahan File</h3>
<pre>
  <code id="log-file">
    git log -- filename.txt
  </code>
</pre>
<button onclick="copyCode('log-file')">Copy</button>

<script>
  function copyCode(id) {
    var code = document.getElementById(id).textContent;
    navigator.clipboard.writeText(code).then(function() {
      alert('Code copied to clipboard!');
    }, function(err) {
      console.error('Could not copy code: ', err);
    });
  }
</script>
