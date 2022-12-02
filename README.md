# Checkpoint
git status
On branch dev

git add .
git status
On branch dev

git status
On branch dev
Your branch is up-to-date with 'origin/dev'.
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

	new file:   Pedro.md
	modified:   token.txt

usuario@us16:~/Desktop/integrador/Checkpoint$ git pull

'''''porque hay conflicto con lo que hay en el servidor''''''
git stash
Saved working directory and index state WIP on dev: 738f01d Agregando nombre en token.txt
HEAD is now at 738f01d Agregando nombre en token.txt

git pull origin dev
From https://github.com/catalinamorenob/Checkpoint
 * branch            dev        -> FETCH_HEAD
Updating 738f01d..09cfb53
Fast-forward
 token.txt | 2 ++
 1 file changed, 2 insertions(+)
nano token.txt
nano PedroMarcano.md
git push origin dev
Everything up-to-date
usuario@us16:~/Desktop/integrador/Checkpoint$ git status
On branch dev
Your branch is up-to-date with 'origin/dev'.
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

	modified:   token.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	PedroMarcano.md

no changes added to commit (use "git add" and/or "git commit -a")
usuario@us16:~/Desktop/integrador/Checkpoint$ git add . 
usuario@us16:~/Desktop/integrador/Checkpoint$ git commit -m pedro      
[dev 462c2c0] pedro
 Committer: usuario <usuario@us16.myguest.virtualbox.org>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 2 files changed, 1 insertion(+), 1 deletion(-)
 create mode 100644 PedroMarcano.md
usuario@us16:~/Desktop/integrador/Checkpoint$ git status
On branch dev
Your branch is ahead of 'origin/dev' by 1 commit.
  (use "git push" to publish your local commits)
nothing to commit, working directory clean
usuario@us16:~/Desktop/integrador/Checkpoint$ clear
[3;J
usuario@us16:~/Desktop/integrador/Checkpoint$ git status
On branch dev
Your branch is ahead of 'origin/dev' by 1 commit.
  (use "git push" to publish your local commits)
nothing to commit, working directory clean
usuario@us16:~/Desktop/integrador/Checkpoint$ git push origin dev
Counting objects: 3, done.
Delta compression using up to 2 threads.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 349 bytes | 0 bytes/s, done.
Total 3 (delta 2), reused 0 (delta 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote: This repository moved. Please use the new location:
remote:   https://github.com/catalinamorenob/checkpoint.git
To https://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@github.com/catalinamorenob/Checkpoint.git
   09cfb53..462c2c0  dev -> dev
usuario@us16:~/Desktop/integrador/Checkpoint$ git checkout PedroMarcano
error: pathspec 'PedroMarcano' did not match any file(s) known to git.
usuario@us16:~/Desktop/integrador/Checkpoint$ git branch pedromarcano
usuario@us16:~/Desktop/integrador/Checkpoint$ git checkout pedromarcano
Switched to branch 'pedromarcano'
usuario@us16:~/Desktop/integrador/Checkpoint$ git status
On branch pedromarcano
nothing to commit, working directory clean
usuario@us16:~/Desktop/integrador/Checkpoint$ ls
CatalinaMoreno.md  Choco.md  PedroMarcano.md  token.txt
usuario@us16:~/Desktop/integrador/Checkpoint$ git status
On branch pedromarcano
nothing to commit, working directory clean
usuario@us16:~/Desktop/integrador/Checkpoint$ ls  
CatalinaMoreno.md  Choco.md  PedroMarcano.md  token.txt
usuario@us16:~/Desktop/integrador/Checkpoint$ mb token.txt clasificados.txt
The program 'mb' is currently not installed. You can install it by typing:
sudo apt install mrbayes
usuario@us16:~/Desktop/integrador/Checkpoint$ mv token.txt clasificados.txt
usuario@us16:~/Desktop/integrador/Checkpoint$ git add .
usuario@us16:~/Desktop/integrador/Checkpoint$ git commit -m pmclasi
[pedromarcano b6797b1] pmclasi
 Committer: usuario <usuario@us16.myguest.virtualbox.org>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 0 insertions(+), 0 deletions(-)
 rename token.txt => clasificados.txt (100%)
usuario@us16:~/Desktop/integrador/Checkpoint$ git push origin dev
Everything up-to-date
usuario@us16:~/Desktop/integrador/Checkpoint$ git status
On branch pedromarcano
nothing to commit, working directory clean
usuario@us16:~/Desktop/integrador/Checkpoint$ ls
CatalinaMoreno.md  Choco.md  clasificados.txt  PedroMarcano.md
usuario@us16:~/Desktop/integrador/Checkpoint$ mv clasificados.txt clasificados
usuario@us16:~/Desktop/integrador/Checkpoint$ ls
CatalinaMoreno.md  Choco.md  clasificados  PedroMarcano.md
usuario@us16:~/Desktop/integrador/Checkpoint$ git add .
usuario@us16:~/Desktop/integrador/Checkpoint$ git status
On branch pedromarcano
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

	renamed:    clasificados.txt -> clasificados

usuario@us16:~/Desktop/integrador/Checkpoint$ git commit -m nuevoCommit
[pedromarcano c0bb7e6] nuevoCommit
 Committer: usuario <usuario@us16.myguest.virtualbox.org>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 0 insertions(+), 0 deletions(-)
 rename clasificados.txt => clasificados (100%)
usuario@us16:~/Desktop/integrador/Checkpoint$ git status
On branch pedromarcano
nothing to commit, working directory clean
usuario@us16:~/Desktop/integrador/Checkpoint$ git status
On branch pedromarcano
nothing to commit, working directory clean
usuario@us16:~/Desktop/integrador/Checkpoint$ git push 
warning: push.default is unset; its implicit value has changed in
Git 2.0 from 'matching' to 'simple'. To squelch this message
and maintain the traditional behavior, use:

  git config --global push.default matching

To squelch this message and adopt the new behavior now, use:

  git config --global push.default simple

When push.default is set to 'matching', git will push local branches
to the remote branches that already exist with the same name.

Since Git 2.0, Git defaults to the more conservative 'simple'
behavior, which only pushes the current branch to the corresponding
remote branch that 'git pull' uses to update the current branch.

See 'git help config' and search for 'push.default' for further information.
(the 'simple' mode was introduced in Git 1.7.11. Use the similar mode
'current' instead of 'simple' if you sometimes use older versions of Git)

fatal: The current branch pedromarcano has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin pedromarcano

usuario@us16:~/Desktop/integrador/Checkpoint$ git push origin pedromarcano
Counting objects: 4, done.
Delta compression using up to 2 threads.
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 467 bytes | 0 bytes/s, done.
Total 4 (delta 2), reused 0 (delta 0)
remote: Resolving deltas: 100% (2/2), completed with 1 local object.
remote: This repository moved. Please use the new location:
remote:   https://github.com/catalinamorenob/checkpoint.git
remote: 
remote: Create a pull request for 'pedromarcano' on GitHub by visiting:
remote:      https://github.com/catalinamorenob/checkpoint/pull/new/pedromarcano
remote: 
To https://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@github.com/catalinamorenob/Checkpoint.git
 * [new branch]      pedromarcano -> pedromarcano
usuario@us16:~/Desktop/integrador/Checkpoint$ git commit -m "Checkpoint finalizado"
On branch pedromarcano
nothing to commit, working directory clean
usuario@us16:~/Desktop/integrador/Checkpoint$ mv clasificados clasificados.txt
usuario@us16:~/Desktop/integrador/Checkpoint$ git add .
usuario@us16:~/Desktop/integrador/Checkpoint$ git commit -m "Checkpoint finalizado"
[pedromarcano 49855a3] Checkpoint finalizado
 Committer: usuario <usuario@us16.myguest.virtualbox.org>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 0 insertions(+), 0 deletions(-)
 rename clasificados => clasificados.txt (100%)
usuario@us16:~/Desktop/integrador/Checkpoint$ git commit -m "Checkpoint finalizado"
On branch pedromarcano
nothing to commit, working directory clean
usuario@us16:~/Desktop/integrador/Checkpoint$ git status                           
On branch pedromarcano
nothing to commit, working directory clean
usuario@us16:~/Desktop/integrador/Checkpoint$ git push origin pedromarcano
Counting objects: 2, done.
Delta compression using up to 2 threads.
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 247 bytes | 0 bytes/s, done.
Total 2 (delta 1), reused 0 (delta 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: This repository moved. Please use the new location:
remote:   https://github.com/catalinamorenob/checkpoint.git
To https://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@github.com/catalinamorenob/Checkpoint.git
   c0bb7e6..49855a3  pedromarcano -> pedromarcano
usuario@us16:~/Desktop/integrador/Checkpoint$ 
