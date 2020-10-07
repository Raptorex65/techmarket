# techmarket
git init . (yeni bir local repository "webshop" oluşturdum)
git add (dosyaları staging area ya yükledim)
git status (dosyaların durumlarını kontrol ettim, hepsi yeşil)
git commit -m  "açıklama" (localden githuba aktardım)
git remote add origin https://.... (githubda oluşturduğum repository adresine tanıttım)
git push -u origin master (bu repository ye push ettim!!)



Değişikliklerin işlenmesi için
PS C:\Users\Selcuk\Desktop\ÖDEVLER\Webshop2> git commit -am
error: switch `m' requires a value
PS C:\Users\Selcuk\Desktop\ÖDEVLER\Webshop2> git commit -am "techmarket css redesign"
[master 1a385fd] techmarket css redesıgn
 4 files changed, 25 insertions(+), 23 deletions(-)
PS C:\Users\Selcuk\Desktop\ÖDEVLER\Webshop2>

GITIGNORE EKLEDİKTEN SONRA LOG:
PS C:\Users\Selcuk\Desktop\ÖDEVLER\Webshop2> touch .gitignore
PS C:\Users\Selcuk\Desktop\ÖDEVLER\Webshop2> git add .gitignore
PS C:\Users\Selcuk\Desktop\ÖDEVLER\Webshop2> git commit -m "message" .gitignore
 1 file changed, 2 insertions(+)
 create mode 100644 .gitignore
PS C:\Users\Selcuk\Desktop\ÖDEVLER\Webshop2> git status
On branch master
Your branch is ahead of 'origin/master' by 2 commits.
  (use "git push" to publish your local commits)

Untracked files:
        Depo.log.1
        Depo.log.2
        Depo.log.3
        Depo.log.4
        Depo.log.5
        Depo.log.6

nothing added to commit but untracked files present (use "git add" to track)
PS C:\Users\Selcuk\Desktop\ÖDEVLER\Webshop2> git push -u origin master
To https://github.com/Raptorex65/techmarket.git
 ! [rejected]        master -> master (fetch first)
error: failed to push some refs to 'https://github.com/Raptorex65/techmarket.git'
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
PS C:\Users\Selcuk\Desktop\ÖDEVLER\Webshop2> git diff
PS C:\Users\Selcuk\Desktop\ÖDEVLER\Webshop2> git pull origin master
remote: Enumerating objects: 7, done.
remote: Counting objects: 100% (7/7), done.
remote: Compressing objects: 100% (6/6), done.
remote: Total 6 (delta 3), reused 0 (delta 0), pack-reused 0
From https://github.com/Raptorex65/techmarket
 * branch            master     -> FETCH_HEAD
   8d5ae57..c12dbb0  master     -> origin/master
Merge made by the 'recursive' strategy.
 README.md | 17 +++++++++++++++++
 1 file changed, 17 insertions(+)
 create mode 100644 README.md
PS C:\Users\Selcuk\Desktop\ÖDEVLER\Webshop2> git push -u origin master
Enumerating objects: 21, done.
Counting objects: 100% (17/17), done.
Delta compression using up to 8 threads
Compressing objects: 100% (10/10), done.
Writing objects: 100% (11/11), 1.21 KiB | 1.21 MiB/s, done.
Total 11 (delta 7), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (7/7), completed with 5 local objects.
To https://github.com/Raptorex65/techmarket.git
   c12dbb0..fb91dd4  master -> master
Branch 'master' set up to track remote branch 'master' from 'origin'.
PS C:\Users\Selcuk\Desktop\ÖDEVLER\Webshop2> git status
On branch master
Your branch is up to date with 'origin/master'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        Deneme.txt
        Depo.log.1
        Depo.log.2
        Depo.log.3
        Depo.log.4
        Depo.log.5
        Depo.log.6

nothing added to commit but untracked files present (use "git add" to track)
PS C:\Users\Selcuk\Desktop\ÖDEVLER\Webshop2>
