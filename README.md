# fullstack-boilerplate

This web-app has no use. It's a playground.


## API (Backend)

Spring Boot (Java)


### Database

MySQL RDMBS (because it comes with *ALL-INKL*)

**_Important_**: *ALL-INKL*-DBs do not support TLS, so do not use it in production!


Here is a capture to demonstrate ```useSSL=false```:

```
.=.......update.
customers.set.ac
tive=1,.created=
'2021-07-25.13:1
7:23',.email='de
v@ivanne.de',.pa
ssword='$2a$10$c
qng9lIb4KzWY1FP9
22g4u0EOzIMmReIx
TBN7TmDkwoFbSA4b
rqei',.updated='
2021-07-25.13:19
:15',.username='
it'.where.custom
erid=27
```

---

## UI (Frontend)

NodeJS React (TypeScript)

Live test: https://reactstrap-ts.netlify.app/


---

## VCS (GitHub)


Remove history:

```console
git checkout --orphan temp-branch
git add .
git commit -m "orphan commit"
git branch -d main
git branch -m temp-branch main
git push -f --set-upstream origin main
```

Add modules:


```console
ivanne@ivanne-desktop:~/Projects/learling/fullstack-boilerplate$ git init
Initialized empty Git repository in /home/ivanne/Projects/learling/fullstack-boilerplate/.git/

ivanne@ivanne-desktop:~/Projects/learling/fullstack-boilerplate$ echo "# fullstack-boilerplate" >> README.md
ivanne@ivanne-desktop:~/Projects/learling/fullstack-boilerplate$ git add README.md
ivanne@ivanne-desktop:~/Projects/learling/fullstack-boilerplate$ git commit -m "first commit"
[master (root-commit) fead118] first commit
 1 file changed, 1 insertion(+)
 create mode 100644 README.md
ivanne@ivanne-desktop:~/Projects/learling/fullstack-boilerplate$ git branch -M main
ivanne@ivanne-desktop:~/Projects/learling/fullstack-boilerplate$ git remote add origin git@github.com:learling/fullstack-boilerplate.git
ivanne@ivanne-desktop:~/Projects/learling/fullstack-boilerplate$ git push -u origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 225 bytes | 225.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To github.com:learling/fullstack-boilerplate.git
 * [new branch]      main -> main
Branch 'main' set up to track remote branch 'main' from 'origin'.
ivanne@ivanne-desktop:~/Projects/learling/fullstack-boilerplate$ git submodule add git@github.com:learling/backend-boilerplate.git backend-boilerplate
Cloning into '/home/ivanne/Projects/learling/fullstack-boilerplate/backend-boilerplate'...
remote: Enumerating objects: 38, done.
remote: Counting objects: 100% (38/38), done.
remote: Compressing objects: 100% (28/28), done.
remote: Total 38 (delta 0), reused 38 (delta 0), pack-reused 0
Receiving objects: 100% (38/38), 55.95 KiB | 690.00 KiB/s, done.
ivanne@ivanne-desktop:~/Projects/learling/fullstack-boilerplate$ git add .
ivanne@ivanne-desktop:~/Projects/learling/fullstack-boilerplate$ git commit -m "add backend submodule"
[main 9c25b22] add backend submodule
 2 files changed, 4 insertions(+)
 create mode 100644 .gitmodules
 create mode 160000 backend-boilerplate
ivanne@ivanne-desktop:~/Projects/learling/fullstack-boilerplate$ git push
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 400 bytes | 400.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To github.com:learling/fullstack-boilerplate.git
   fead118..9c25b22  main -> main
ivanne@ivanne-desktop:~/Projects/learling/fullstack-boilerplate$ git submodule add git@github.com:learling/frontend-boilerplate.git frontend-boilerplate
Cloning into '/home/ivanne/Projects/learling/fullstack-boilerplate/frontend-boilerplate'...
remote: Enumerating objects: 48, done.
remote: Counting objects: 100% (48/48), done.
remote: Compressing objects: 100% (32/32), done.
remote: Total 48 (delta 11), reused 48 (delta 11), pack-reused 0
Receiving objects: 100% (48/48), 375.52 KiB | 293.00 KiB/s, done.
Resolving deltas: 100% (11/11), done.
ivanne@ivanne-desktop:~/Projects/learling/fullstack-boilerplate$ git add .
ivanne@ivanne-desktop:~/Projects/learling/fullstack-boilerplate$ git commit -m "add frontend submodule"
[main 09c54db] add frontend submodule
 2 files changed, 4 insertions(+)
 create mode 160000 frontend-boilerplate
ivanne@ivanne-desktop:~/Projects/learling/fullstack-boilerplate$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 453 bytes | 453.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To github.com:learling/fullstack-boilerplate.git
   9c25b22..09c54db  main -> main
ivanne@ivanne-desktop:~/Projects/learling/fullstack-boilerplate$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
    modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")
ivanne@ivanne-desktop:~/Projects/learling/fullstack-boilerplate$ git add .
ivanne@ivanne-desktop:~/Projects/learling/fullstack-boilerplate$ git commit -m "add md content"
[main d43b3c7] add md content
 1 file changed, 133 insertions(+)
ivanne@ivanne-desktop:~/Projects/learling/fullstack-boilerplate$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 1.18 KiB | 1.18 MiB/s, done.
Total 3 (delta 1), reused 0 (delta 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To github.com:learling/fullstack-boilerplate.git
   09c54db..d43b3c7  main -> main
```

