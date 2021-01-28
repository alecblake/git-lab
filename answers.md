1.PS C:\Users\alecb> git --version
git version 2.30.0.windows.2
PS C:\Users\alecb>

2. Windows PowerShell
Copyright (C) Microsoft Corporation. All rights reserved.
Try the new cross-platform PowerShell https://aka.ms/pscore6
PS C:\Users\alecb> cd Documents
PS C:\Users\alecb\Documents> cd cs2400
PS C:\Users\alecb\Documents\cs2400> mkdir git-lab
Directory : C:\Users\alecb\Documents\cs2400
Mode	LastWriteTime	Length Name
d		1/27/2021	4:14 PM	git-lab
PS C:\Users\alecb\Documents\cs2400> cd git-lab
PS C:\Users\alecb\Documents\cs2400\git-lab> echo >> README.md
PS C:\Users\alecb\Documents\cs2400\git-lab> echo » answers.md
PS C:\Users\alecb\Documents\cs2400\git-lab> git config -global user.name
PS C:\Users\alecb\Documents\cs2400\git-lab> git config -global user.email
PS C:\Users\alecb\Documents\cs2400\git-lab> git config -list
diff.astextplain.textconv=astextplain
filter.lfs.clean-git-lfs clean -- Xf
filter.Ifs.smudge=git-lfs smudge -- Xf
filter.lfs.process=git-lfs filter-process
filter.Ifs.required-true
http.sslbackend=openssl
http.sslcainfo=C:/Program Files/Git/mingw64/ssl/certs/ca-bundle.crt
core.autocrlf-true
core.fscache=true
core.symlinks=false
pull.rebase-false
credential.helper=manager-core
credential.https ://dev.azure.com.usehttppath=true
init.defaultbranch-master
filter.Ifs.smudge=git-lfs smudge -- Xf
filter.lfs.process=git-lfs filter-process
filter.Ifs.required-true
filter.lfs.clean=git-lfs clean -- Xf
user.name=Alec Blake
user.email-ab587817@ohio.edu
PS C:\Users\alecb\Documents\cs2400\git-lab>

3.5S C:\Usens\alecb> git command -help
jit: 'command' is not a git command. See 'git --help'.
5S C:\Users\alecb> git -help
jsage: git [--version] [--help] [-C <path>] [-c <name>-<value>]
[--exec-path[-<path>]] [--html-path] [--man-path] [--info-path]
[-p I --paginate | -P | --no-pager] [--no-replace-objects] [--bare] [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>] <command> [<args>]
rhese are common Git commands used in various situations:
start a working area (see also: git help tutorial)
clone	Clone a repository into a new directory
init	Create an empty Git repository or reinitialize an existing one
tfork on the current add mv
restore
rm
sparse-checkout
change (see also: git help everyday)
Add file contents to the index
Move or rename a file, a directory, or a symlink
Restore working tree files
Remove files from the working tree and from the index
Initialize and modify the sparse-checkout
examine the history bisect diff grep log show status
and state (see also: git help revisions)
Use binary search to find the commit that introduced a bug
Show changes between commits, commit and working tree, etc
Print lines matching a pattern
Show commit logs
Show various types of objects
Show the working tree status
»row, mark and tweak your common history
branch	List, create, or delete branches
commit	Record changes to the repository
merge	loin two or more development histories together
rebase	Reapply commits on top of another base tip
reset	Reset current HEAD to the specified state
switch	Switch branches
tag	Create, list, delete or verify a tag object signed	with	GPG
:ollaborate (see also: git help workflows)
fetch	Download objects and refs from another repository
pull	Fetch from and integrate with another repository or	a	local branch
push	Update remote refs along with associated objects
'git help -a* and 'git help -g* list available subcommands and some :oncept guides. See 'git help <comraand>' or 'git help <concept>'
Co read about a specific subcommand or concept, iee 'git help git' for an overview of the system.
3S C:\Users\alecb>

4.PS C:\Users\alecb\Documents\cs2400\git-lab> git init
Initialized empty Git repository in C:/Users/alecb/Documents/cs2400/git-lab/.git/ PS C:\Users\alecb\Documents\cs2400\git-lab> echo >> README.md PS C:\Users\alecb\Documents\cs2400\git-lab> git status On branch master
Mo commits yet
Untracked files:
(use "git add <file>..." to include in what will be committed)
nothing added to commit but untracked files present (use "git add" to track) PS C:\Users\alecb\Documents\cs2400\git-lab>

5. nothing added to commit but untracked files present (use "git add" to track) PS C:\Users\alecb\Documents\cs2400\git-lab> git add README.md PS C:\Users\alecb\Documents\cs2400\git-lab> git .add README.md git: '.add' is not a git command. See 'git --help'.
The most similar command is add
PS C:\Users\alecb\Documents\cs2400\git-lab> git status On branch master
No commits yet
Changes to be committed:
(use "git rm --cached <file>..." to unstage)
Untracked files:
(use "git add <file>..." to include in what will be committed)
PS C:\Users\alecb\Documents\cs2400\git-lab>

6. PS C:\Users\alecb\Documents\cs2400\git-lab> git add answers.md PS C:\Users\alecb\Documents\cs2400\git-lab> git status )n branch master
No commits yet
Changes to be committed:
(use "git rm --cached <file>..." to unstage)
PS C:\Users\alecb\Documents\cs2400\git-lab>

7. PS C:\Users\alecb\Documents\cs2400\git-lab> git commit -m [master (root-commit) 56b7elf] Initial commit 2 files changed, 0 insertions(+), 0 deletions(-) create mode 100644 README.md create mode 100644 answers.md PS C:\Users\alecb\Documents\cs2400\git-lab> git status On branch master
nothing to commit, working tree clean
PS C:\Users\alecb\Documents\cs2400\git-lab>

8. PS C:\Usens\alecb\Documents\cs2400\git-lab> git log
commit 56b7elfdd6fa6b8e77fa66c01670024407bc7ad8 (HEAD -> master)
Author: Alec Blake <ab587817@ohio.edu>
Date:	Wed Dan 27 17:10:13 2021 -0500
Initial commit
PS C:\Users\alecb\Documents\cs2400\git-lab>

9.Initial commit
PS C:\Users\alecb\Documents\cs2400\git-lab> git remote add origin http://github.com/alecblake/git-lab.git
PS C:\Users\alecb\Documents\cs2400\git-lab> git branch -M main
PS C:\Users\alecb\Documents\cs2400\git-lab> git push -u origin main
info: please complete authentication in your browser...
warning: redirecting to https://github.com/alecblake/git-lab.git/
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads Compressing objects: 100% (3/3), done.
Writing objects: 100% (4/4), 293 bytes | 146.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0 To http://github.com/alecblake/git-lab.git * [new branch]	main -> main
Branch 'main' set up to track remote branch 'main' from 'origin*.

10. Alec Blake
alecblake
ab587817@ohio.edu
Answers located in answers.md

11.PS C:\Users\alecb\Documents\cs2400\git-lab> git push
warning: redirecting to https://github.com/alecblake/git-lab.git/
To http://github.com/alecblake/git-lab.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'http://github.com/alecblake/git-lab.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
PS C:\Users\alecb\Documents\cs2400\git-lab>

12. 




