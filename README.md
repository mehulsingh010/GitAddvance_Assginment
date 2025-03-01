Commands Used

Mehul@hppavilion MINGW64 /d/GitAdvance_Assg_Personal (MehulSingh)
$ echo "This is reset soft command" >> reset.txt

Mehul@hppavilion MINGW64 /d/GitAdvance_Assg_Personal (MehulSingh)
$ git add reset.txt
warning: in the working copy of 'reset.txt', LF will be replaced by CRLF the next time Git touches it

Mehul@hppavilion MINGW64 /d/GitAdvance_Assg_Personal (MehulSingh)
$ git commit -m "add reset.txt file"
[MehulSingh fff07c5] add reset.txt file
 1 file changed, 1 insertion(+)
 create mode 100644 reset.txt

Mehul@hppavilion MINGW64 /d/GitAdvance_Assg_Personal (MehulSingh)
$ git status
On branch MehulSingh
Your branch is ahead of 'origin/MehulSingh' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

Mehul@hppavilion MINGW64 /d/GitAdvance_Assg_Personal (MehulSingh)
$ git log
commit fff07c54f6a5d70529b5c9a289eb9f3d70023818 (HEAD -> MehulSingh)
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Tue Jan 7 00:28:30 2025 +0530

    add reset.txt file

commit 6a106767874cafc748e1d48e54c55759cfe5e9cf (origin/MehulSingh)
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 23:39:38 2025 +0530

    rename of file

commit 28a36c9fc52b4909a974ed2cf2af59b7fc60b947
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 22:44:21 2025 +0530

    add original file

commit f3ebf670372491d540fa35cc7a1280f4560a1a0d
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 22:42:29 2025 +0530

    delete original.txt

commit cc42f3dfe9b50925d96cbd08d627e0f939572653
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 22:16:11 2025 +0530

    Add original file

commit 77647ddac0987a14be02c2f28513e6f0145060ef (backup/MehulSingh)
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 18:37:07 2025 +0530

    add demo in question5.txt file

commit adce1003161fec7ebc4a58d687fb4ddda30dd661
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 18:14:52 2025 +0530

    add q1 q2 q3 q4 q5 q6

commit 6ca5bb0907cc66d9da579bcad63e71a6c2444670
Merge: e767616 9e7db8f
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 13:04:00 2025 +0530

    Merge branch 'branch1'

commit e767616bdbec2d2498c52c79ba045aaec818741e
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 13:03:46 2025 +0530

    Delete conflict.txt in main branch

commit 9e7db8fcdefe886c28d6075cd4877222726fc36c

Mehul@hppavilion MINGW64 /d/GitAdvance_Assg_Personal (MehulSingh)
$ git reset --soft HEAD~1

Mehul@hppavilion MINGW64 /d/GitAdvance_Assg_Personal (MehulSingh)
$ git status
On branch MehulSingh
Your branch is up to date with 'origin/MehulSingh'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   reset.txt


Mehul@hppavilion MINGW64 /d/GitAdvance_Assg_Personal (MehulSingh)
$ cat reset.txt
This is reset soft command

Mehul@hppavilion MINGW64 /d/GitAdvance_Assg_Personal (MehulSingh)
$ git commit -m "add reset.txt file"
[MehulSingh b55e133] add reset.txt file
 1 file changed, 1 insertion(+)
 create mode 100644 reset.txt

Mehul@hppavilion MINGW64 /d/GitAdvance_Assg_Personal (MehulSingh)
$ git status
On branch MehulSingh
Your branch is ahead of 'origin/MehulSingh' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

Mehul@hppavilion MINGW64 /d/GitAdvance_Assg_Personal (MehulSingh)
$ git reset --hard HEAD~1
HEAD is now at 6a10676 rename of file

Mehul@hppavilion MINGW64 /d/GitAdvance_Assg_Personal (MehulSingh)
$ git log
commit 6a106767874cafc748e1d48e54c55759cfe5e9cf (HEAD -> MehulSingh, origin/MehulSingh)
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 23:39:38 2025 +0530

    rename of file

commit 28a36c9fc52b4909a974ed2cf2af59b7fc60b947
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 22:44:21 2025 +0530

    add original file

commit f3ebf670372491d540fa35cc7a1280f4560a1a0d
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 22:42:29 2025 +0530

    delete original.txt

commit cc42f3dfe9b50925d96cbd08d627e0f939572653
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 22:16:11 2025 +0530

    Add original file

commit 77647ddac0987a14be02c2f28513e6f0145060ef (backup/MehulSingh)
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 18:37:07 2025 +0530

    add demo in question5.txt file

commit adce1003161fec7ebc4a58d687fb4ddda30dd661
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 18:14:52 2025 +0530

    add q1 q2 q3 q4 q5 q6

commit 6ca5bb0907cc66d9da579bcad63e71a6c2444670
Merge: e767616 9e7db8f
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 13:04:00 2025 +0530

    Merge branch 'branch1'

commit e767616bdbec2d2498c52c79ba045aaec818741e
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 13:03:46 2025 +0530

    Delete conflict.txt in main branch

commit 9e7db8fcdefe886c28d6075cd4877222726fc36c
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 12:59:32 2025 +0530

    update the confllict.txt

commit a015aba4a50f1cf9731a1dc505973326b9393919

Mehul@hppavilion MINGW64 /d/GitAdvance_Assg_Personal (MehulSingh)
$ git status
On branch MehulSingh
Your branch is up to date with 'origin/MehulSingh'.

nothing to commit, working tree clean

Mehul@hppavilion MINGW64 /d/GitAdvance_Assg_Personal (MehulSingh)
$ cat reset.txt
cat: reset.txt: No such file or directory

Mehul@hppavilion MINGW64 /d/GitAdvance_Assg_Personal (MehulSingh)
$ touch reset_soft_hard.txt

>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>

Mehul@hppavilion MINGW64 /d/GitAdvance_Assg_Personal (MehulSingh)
$ git stash
Saved working directory and index state WIP on MehulSingh: 353e837 Add reset_doft_hard.txt file

Mehul@hppavilion MINGW64 /d/GitAdvance_Assg_Personal (MehulSingh)
$ git stash list
stash@{0}: WIP on MehulSingh: 353e837 Add reset_doft_hard.txt file

Mehul@hppavilion MINGW64 /d/GitAdvance_Assg_Personal (MehulSingh)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

Mehul@hppavilion MINGW64 /d/GitAdvance_Assg_Personal (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

Mehul@hppavilion MINGW64 /d/GitAdvance_Assg_Personal (main)
$ git checkout MehulSingh
Switched to branch 'MehulSingh'
Your branch is ahead of 'origin/MehulSingh' by 1 commit.
  (use "git push" to publish your local commits)

Mehul@hppavilion MINGW64 /d/GitAdvance_Assg_Personal (MehulSingh)
$ cat change.txt
cat: change.txt: No such file or directory

Mehul@hppavilion MINGW64 /d/GitAdvance_Assg_Personal (MehulSingh)
$ git stash pop
On branch MehulSingh
Your branch is ahead of 'origin/MehulSingh' by 1 commit.
  (use "git push" to publish your local commits)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   change.txt

Dropped refs/stash@{0} (4a14c23c520d6603a4b2a2ce23d98a83b3179bcb)


>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>.......

Mehul@hppavilion MINGW64 /d/GitAdvance_Assg_Personal (fetch)
$ git checkout NewBranch
Switched to branch 'NewBranch'
Your branch is up to date with 'origin/NewBranch'.

Mehul@hppavilion MINGW64 /d/GitAdvance_Assg_Personal (NewBranch)
$ git ls -files
git: 'ls' is not a git command. See 'git --help'.

The most similar command is
        lfs

Mehul@hppavilion MINGW64 /d/GitAdvance_Assg_Personal (NewBranch)
$ git ls-files
one/f1.txt
one/f2.txt
two/ecollege.txt
two/hschool.txt
two/school.txt

Mehul@hppavilion MINGW64 /d/GitAdvance_Assg_Personal (NewBranch)
$ git cherry-pick b5de88a26f4212b902a6ac69592db8531c698b75
[NewBranch 4185fda] Add reset_doft_hard.txt file
 Date: Tue Jan 7 01:19:41 2025 +0530
 1 file changed, 195 insertions(+)
 create mode 100644 reset_soft_hard.txt

Mehul@hppavilion MINGW64 /d/GitAdvance_Assg_Personal (NewBranch)
$ git status
On branch NewBranch
Your branch is ahead of 'origin/NewBranch' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

Mehul@hppavilion MINGW64 /d/GitAdvance_Assg_Personal (NewBranch)
$ git log
commit 4185fdabbdcb61a6241acec98bd48dbe10d7cffb (HEAD -> NewBranch)
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Tue Jan 7 01:19:41 2025 +0530

    Add reset_doft_hard.txt file

commit e767616bdbec2d2498c52c79ba045aaec818741e (origin/NewBranch)
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 13:03:46 2025 +0530

    Delete conflict.txt in main branch

commit a015aba4a50f1cf9731a1dc505973326b9393919
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 12:54:03 2025 +0530

    add conflict.txt with content

commit a355972b2e51073a7ce0782a69024d9db2f96588
Merge: 7b6d665 9fc05af
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 12:42:24 2025 +0530

    Merge branch 'branch1'

commit 9fc05afd122d47aff7f5d8e33a512fa5618db813
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 12:35:07 2025 +0530

    add Engineering college info

commit 7b6d66564f885a3d41168b42e4e41ce7f4db555c
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 12:29:01 2025 +0530

    Add High Schhol info

commit b40dc3ca23cef44a2d82dd54c48f08bbd5844eda
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 12:16:19 2025 +0530

    initial commit add two folders one and two

Mehul@hppavilion MINGW64 /d/GitAdvance_Assg_Personal (NewBranch)
$ git ls-files
one/f1.txt
one/f2.txt
reset_soft_hard.txt
two/ecollege.txt
two/hschool.txt
two/school.txt

Mehul@hppavilion MINGW64 /d/GitAdvance_Assg_Personal (NewBranch)
$ git branch
  MehulSingh
* NewBranch
  branch1
  branch2
  fetch
  fix/bug
  main

Mehul@hppavilion MINGW64 /d/GitAdvance_Assg_Personal (NewBranch)
$ git ls-files
one/f1.txt
one/f2.txt
reset_soft_hard.txt
two/ecollege.txt
two/hschool.txt
two/school.txt

Mehul@hppavilion MINGW64 /d/GitAdvance_Assg_Personal (NewBranch)
$ touch file.txt

Mehul@hppavilion MINGW64 /d/GitAdvance_Assg_Personal (NewBranch)
$ echo "This files used for adding new commit into latest commit made" > file.txt

Mehul@hppavilion MINGW64 /d/GitAdvance_Assg_Personal (NewBranch)
$ cat file.txt
This files used for adding new commit into latest commit made

Mehul@hppavilion MINGW64 /d/GitAdvance_Assg_Personal (NewBranch)
$ git astatus
git: 'astatus' is not a git command. See 'git --help'.

The most similar command is
        status

Mehul@hppavilion MINGW64 /d/GitAdvance_Assg_Personal (NewBranch)
$ git status
On branch NewBranch
Your branch is ahead of 'origin/NewBranch' by 1 commit.
  (use "git push" to publish your local commits)

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        file.txt

nothing added to commit but untracked files present (use "git add" to track)

Mehul@hppavilion MINGW64 /d/GitAdvance_Assg_Personal (NewBranch)
$ git add .
warning: in the working copy of 'file.txt', LF will be replaced by CRLF the next time Git touches it

Mehul@hppavilion MINGW64 /d/GitAdvance_Assg_Personal (NewBranch)
$ git status
On branch NewBranch
Your branch is ahead of 'origin/NewBranch' by 1 commit.
  (use "git push" to publish your local commits)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   file.txt


Mehul@hppavilion MINGW64 /d/GitAdvance_Assg_Personal (NewBranch)
$ git log
commit 4185fdabbdcb61a6241acec98bd48dbe10d7cffb (HEAD -> NewBranch)
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Tue Jan 7 01:19:41 2025 +0530

    Add reset_doft_hard.txt file

commit e767616bdbec2d2498c52c79ba045aaec818741e (origin/NewBranch)
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 13:03:46 2025 +0530

    Delete conflict.txt in main branch

commit a015aba4a50f1cf9731a1dc505973326b9393919
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 12:54:03 2025 +0530

    add conflict.txt with content

commit a355972b2e51073a7ce0782a69024d9db2f96588
Merge: 7b6d665 9fc05af
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 12:42:24 2025 +0530

    Merge branch 'branch1'

commit 9fc05afd122d47aff7f5d8e33a512fa5618db813
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 12:35:07 2025 +0530

    add Engineering college info

commit 7b6d66564f885a3d41168b42e4e41ce7f4db555c
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 12:29:01 2025 +0530

    Add High Schhol info

commit b40dc3ca23cef44a2d82dd54c48f08bbd5844eda
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 12:16:19 2025 +0530

    initial commit add two folders one and two

Mehul@hppavilion MINGW64 /d/GitAdvance_Assg_Personal (NewBranch)
$ git commit --amend -m "add changes to latest commit"
[NewBranch 3ba9414] add changes to latest commit
 Date: Tue Jan 7 01:19:41 2025 +0530
 2 files changed, 196 insertions(+)
 create mode 100644 file.txt
 create mode 100644 reset_soft_hard.txt

Mehul@hppavilion MINGW64 /d/GitAdvance_Assg_Personal (NewBranch)
$ git log
commit 3ba9414e9c966113cefd0d1fd2d5b5b3f7c8e7ef (HEAD -> NewBranch)
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Tue Jan 7 01:19:41 2025 +0530

    add changes to latest commit

commit e767616bdbec2d2498c52c79ba045aaec818741e (origin/NewBranch)
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 13:03:46 2025 +0530

    Delete conflict.txt in main branch

commit a015aba4a50f1cf9731a1dc505973326b9393919
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 12:54:03 2025 +0530

    add conflict.txt with content

commit a355972b2e51073a7ce0782a69024d9db2f96588
Merge: 7b6d665 9fc05af
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 12:42:24 2025 +0530

    Merge branch 'branch1'

commit 9fc05afd122d47aff7f5d8e33a512fa5618db813
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 12:35:07 2025 +0530

    add Engineering college info

commit 7b6d66564f885a3d41168b42e4e41ce7f4db555c
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 12:29:01 2025 +0530

    Add High Schhol info

commit b40dc3ca23cef44a2d82dd54c48f08bbd5844eda
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 12:16:19 2025 +0530

    initial commit add two folders one and two

>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>

Mehul@hppavilion MINGW64 /d/GitAdvance_Assg_Personal (NewBranch)
$ git checkout branch1
Switched to branch 'branch1'
Your branch is up to date with 'backup/branch1'.

Mehul@hppavilion MINGW64 /d/GitAdvance_Assg_Personal (branch1)
$ git log
commit 85ab6eddf3f745bf1de971fc1a84d864e8b3db4a (HEAD -> branch1, origin/branch1, backup/branch1)
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 15:07:56 2025 +0530

    add conflict in branch1

commit 9e7db8fcdefe886c28d6075cd4877222726fc36c
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 12:59:32 2025 +0530

    update the confllict.txt

commit 9fc05afd122d47aff7f5d8e33a512fa5618db813
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 12:35:07 2025 +0530

    add Engineering college info

commit b40dc3ca23cef44a2d82dd54c48f08bbd5844eda
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 12:16:19 2025 +0530

    initial commit add two folders one and two

Mehul@hppavilion MINGW64 /d/GitAdvance_Assg_Personal (branch1)
$ git ls-files
conflict.txt
one/f1.txt
one/f2.txt
two/ecollege.txt
two/school.txt

Mehul@hppavilion MINGW64 /d/GitAdvance_Assg_Personal (branch1)
$ git rebase MehulSingh
Successfully rebased and updated refs/heads/branch1.

Mehul@hppavilion MINGW64 /d/GitAdvance_Assg_Personal (branch1)
$ git ls-files
Mehul/question1.txt
Mehul/question2.txt
Mehul/question3.txt
Mehul/question4.txt
Mehul/question5.txt
Mehul/question6.txt
change.txt
conflict.txt
new.txt
one/f1.txt
one/f2.txt
reset_soft_hard.txt
stashpop.txt
two/ecollege.txt
two/hschool.txt
two/school.txt

Mehul@hppavilion MINGW64 /d/GitAdvance_Assg_Personal (branch1)
$ git log
commit aa721237080f862bc593463d4cb6cc0c2dd23a76 (HEAD -> branch1)
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 15:07:56 2025 +0530

    add conflict in branch1

commit bf0bb67da352270455787f6390223ff882420f36 (origin/MehulSingh, MehulSingh)
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Tue Jan 7 01:58:03 2025 +0530

    add stash pop demo file

commit 84273edc3a4bde6efe4b0a802b4c40413eaf064a
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Tue Jan 7 01:55:54 2025 +0530

    use Of Stash and Stash pop after add and modify made in file

commit 6a106767874cafc748e1d48e54c55759cfe5e9cf
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 23:39:38 2025 +0530

    rename of file

commit 28a36c9fc52b4909a974ed2cf2af59b7fc60b947
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 22:44:21 2025 +0530

    add original file

commit f3ebf670372491d540fa35cc7a1280f4560a1a0d
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 22:42:29 2025 +0530

    delete original.txt

commit cc42f3dfe9b50925d96cbd08d627e0f939572653
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 22:16:11 2025 +0530

    Add original file

commit 77647ddac0987a14be02c2f28513e6f0145060ef (backup/MehulSingh)
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 18:37:07 2025 +0530

    add demo in question5.txt file

commit adce1003161fec7ebc4a58d687fb4ddda30dd661
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 18:14:52 2025 +0530

    add q1 q2 q3 q4 q5 q6

commit 6ca5bb0907cc66d9da579bcad63e71a6c2444670
Merge: e767616 9e7db8f
