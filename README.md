# gitCheatSheet
Commands for not wrecking everything when using git (prevention of wrecking not guaranteed).

##General Settings
###Change username and e-mail
git config user.name ["your username"] </br>
git config user.email ["your email"]

##Commiting Work
###Committing just some files
git commit [file names]
###Committing all files
git add -A</br>
git commit -m ["Your commit message"]

##Undoing things
###Roll back changes that have been pushed
git push -f origin [SHA of commit you want to roll back to]:master
###Undo all unstaged changes
git checkout -- .

##Tagging
###Tagging a commit
git tag -a [the tag name] [the commit hash] -m "[the tag message]"
###Pushing a tag
git push --tags origin master

##Merging
###Force merge to master using all changes from branch
git checkout [branch to become master]</br>
git merge -s ours master</br>
git checkout master</br>
git merge [branch to become master]</br>

##Branching
###Create a branch locally
git checkout -b [name-of-branch]</br>
###Add branch to remote
git push origin [name-of-branch]
###Merge master into your branch
git checkout [name-of-branch]
git fetch origin </br>
git merge origin/master </br>