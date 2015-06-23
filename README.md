# gitCheatSheet
commands for not wrecking everything when using git.

##General Settings
###Change username and e-mail
git config user.name ["your username"] </br>
git config user.email ["your email"]

##Commiting Work
###Committing just some files
git commit [file names]
###Committing all files
git add -A
git commit -m ["Your commit message"]

##Undoing things
###Roll back changes that have been pushed
git push -f origin [SHA of commit you want to roll back to]:master
###Undo all unstaged changes
git checkout -- .