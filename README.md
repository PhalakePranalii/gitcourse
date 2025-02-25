D:\DotNet Code\gitCourse> git clone https://github.com/PhalakePranalii/gitcourse.git
Cloning into 'gitcourse'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Receiving objects: 100% (3/3), done.

D:\DotNet Code\gitCourse>cd gitCourse

D:\DotNet Code\gitCourse\gitcourse>git remote -v
origin  https://github.com/PhalakePranalii/gitcourse.git (fetch)
origin  https://github.com/PhalakePranalii/gitcourse.git (push)

D:\DotNet Code\gitCourse\gitcourse>echo firstFile > firstFile.txt

D:\DotNet Code\gitCourse\gitcourse>git add -h
usage: git add [<options>] [--] <pathspec>...

    -n, --[no-]dry-run    dry run
    -v, --[no-]verbose    be verbose

    -i, --[no-]interactive
                          interactive picking
    -p, --[no-]patch      select hunks interactively
    -e, --[no-]edit       edit current diff and apply
    -f, --[no-]force      allow adding otherwise ignored files
    -u, --[no-]update     update tracked files
    --[no-]renormalize    renormalize EOL of tracked files (implies -u)
    -N, --[no-]intent-to-add
                          record only the fact that the path will be added later
    -A, --[no-]all        add changes from all tracked and untracked files
    --[no-]ignore-removal ignore paths removed in the working tree (same as --no-all)
    --[no-]refresh        don't add, only refresh the index
    --[no-]ignore-errors  just skip files which cannot be added because of errors
    --[no-]ignore-missing check if - even missing - files are ignored in dry run
    --[no-]sparse         allow updating entries outside of the sparse-checkout cone
    --[no-]chmod (+|-)x   override the executable bit of the listed files
    --[no-]pathspec-from-file <file>
                          read pathspec from file
    --[no-]pathspec-file-nul
                          with --pathspec-from-file, pathspec elements are separated with NUL character


D:\DotNet Code\gitCourse\gitcourse>git add .

D:\DotNet Code\gitCourse\gitcourse>git commit -m "Adding a first test file"
[main 2581764] Adding a first test file
 1 file changed, 1 insertion(+)
 create mode 100644 firstFile.txt

D:\DotNet Code\gitCourse\gitcourse>git branch
* main

D:\DotNet Code\gitCourse\gitcourse>get log
'get' is not recognized as an internal or external command,
operable program or batch file.

D:\DotNet Code\gitCourse\gitcourse>git log
commit 258176422f7e051453657d7a69ccf64d32f9f1fc (HEAD -> main)
Author: phalakepranali523@gmail.com <phalakepranali523@gmail.com>
Date:   Tue Feb 25 11:07:38 2025 +0530

    Adding a first test file

commit 5a3953bca1e626bb02e063a43628af64cb6825f1 (origin/main, origin/HEAD)
Author: PhalakePranalii <114426851+PhalakePranalii@users.noreply.github.com>
Date:   Tue Feb 25 11:02:42 2025 +0530

    Create code

D:\DotNet Code\gitCourse\gitcourse>echo staged > staged.txt

D:\DotNet Code\gitCourse\gitcourse>echo unStaged > unStaged.txt

D:\DotNet Code\gitCourse\gitcourse>git status
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        staged.txt
        unStaged.txt

nothing added to commit but untracked files present (use "git add" to track)

D:\DotNet Code\gitCourse\gitcourse>git add staged.txt

D:\DotNet Code\gitCourse\gitcourse>git status
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   staged.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        unStaged.txt


D:\DotNet Code\gitCourse\gitcourse>git commit -m "added one staged file of txt type"
[main aef8325] added one staged file of txt type
 1 file changed, 1 insertion(+)
 create mode 100644 staged.txt

D:\DotNet Code\gitCourse\gitcourse>git branch
* main

D:\DotNet Code\gitCourse\gitcourse>git log
commit aef8325e24728ad3b6d49238cc3710855d29230d (HEAD -> main)
Author: phalakepranali523@gmail.com <phalakepranali523@gmail.com>
Date:   Tue Feb 25 11:16:29 2025 +0530

    added one staged file of txt type

commit 258176422f7e051453657d7a69ccf64d32f9f1fc
Author: phalakepranali523@gmail.com <phalakepranali523@gmail.com>
Date:   Tue Feb 25 11:07:38 2025 +0530

    Adding a first test file

commit 5a3953bca1e626bb02e063a43628af64cb6825f1 (origin/main, origin/HEAD)
Author: PhalakePranalii <114426851+PhalakePranalii@users.noreply.github.com>
Date:   Tue Feb 25 11:02:42 2025 +0530

    Create code

D:\DotNet Code\gitCourse\gitcourse>git push
remote: Invalid username or password.
fatal: Authentication failed for 'https://github.com/PhalakePranalii/gitcourse.git/'

D:\DotNet Code\gitCourse\gitcourse>git push origin main
fatal: User cancelled dialog.
Username for 'https://github.com': PhalakePranalii
Password for 'https://PhalakePranalii@github.com':
remote: Support for password authentication was removed on August 13, 2021.
remote: Please see https://docs.github.com/get-started/getting-started-with-git/about-remote-repositories#cloning-with-https-urls for information on currently recommended modes of authentication.
fatal: Authentication failed for 'https://github.com/PhalakePranalii/gitcourse.git/'

D:\DotNet Code\gitCourse\gitcourse>
