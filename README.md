# ${{\color{red}GIT-NOTE}}$
![Git Indexing](https://static.javatpoint.com/tutorial/git/images/git-index.png)
1. create a folder, and in the path of the folder, just enter cmd and click, it opens the terminal with the path of the folder.
2. Then in terminal, enter **${{\color{orange}code\ .}}$**, it opens the project in vs code.
3. **${{\color{orange}git\ init}}$** - to initialize a git repositoty in the project.
4. first project is in working directory -> git add -> goes to staging area -> git commit -> repositoty
5. **${{\color{orange}git\ status}}$** - gives information whether any files are added or not added in staging area and also commited or not.
6. if a folder contains index.html file, then **${{\color{orange}git \ add\ index.html}}$** adds index.html to the staging area.
7. **${{\color{orange}git\ commit\ -m\ "any message regarding changes made"}}$**, pushes from staging area to repository.
8. to add all newly added files or changes: **${{\color{orange}git\ add\ .}}$**(but if any files are deleted, it wont update in repo)
9. to overcome "git add ." issue we have **${{\color{orange}git\ add\ -A}}$**, it performs all changes even deletion too.
10. to undo the mistakes made in a file, lets say in index.html,we can use **${{\color{orange}git\ checkout\ index.html}}$**
11. **${{\color{orange}git\ diff}}$**, to see all the changes made with respect to commited code.
12. **${{\color{orange}git\ diff\ index.html}}$** only shows the changes made in index.html file.
13. **${{\color{orange};\ wq}}$** to get out of the git editor.
14. **${{\color{orange}git\ diff\ --staged}}$**, to see the changes in staging area.
15. **${{\color{orange}git\ diff\ HEAD}}$**, to see the changes in commit area.
16. **${{\color{orange}git\ log}}$**, contains entire info or history of all the commits made(contains author name, date when commit made, commit message).
17. **${{\color{orange}git\ log\ -p\ -n}}$**, where n means last n(numeric value) commits.
18. **${{\color{orange}git\ rm\ index.html}}$**, deletes index.html file.
19. **${{\color{orange}git\ rm\ --cached\ index.html}}$**, reverts index.html from staging area to working directory.
20. **${{\color{orange}git\ branch\ --list}}$**, lists all the branches.
21. **${{\color{orange}git\ branch\ branch-name}}$**, to create a new branch from the current branch.
22. **${{\color{orange}git\ checkout\ branch-name}}$**, to jump to newly created branch branch-name.
23. changes made in one branch wont be visible in its previous branches, if not merged.
24. **${{\color{orange}git\ branch\ -d\ branch-name}}$**, to delete a branch.
25. **${{\color{orange}git\ merge\ branch-name}}$**, to merge a branch with branch-name in the current branch.
26. **${{\color{orange}git\ checkout\ -b\ branch-name}}$**, to create and checkout branch at the same time.
27. **${{\color{orange}git\ commit\ -a\ -m\ message}}$**, to add and commit at the same time.
28. **${{\color{orange}git\ branch\ -M\ new-branch-name}}$**, to rename the branch name.
29. **${{\color{orange}git\ push\ -u\ origin\ branch-name}}$**, to push in the specified branch.
30. **${{\color{orange}git\ push\ -u\ -f\ origin\ branch-name}}$**, for force push.
31. **${{\color{orange}git\ remote\ add\ origin\ github-repo-remote-URL}}$**,to add the path of remote repository in github.
32. **${{\color{orange}git\ clone\ github-repo-remote-URL}}$**, to clone or copy the entire project from main branch of github to the path of the folder specified in bash. 
33. Git clone means making a copy of the repository on the local system while git fork means copying a repository on the remote server itself i.e on the github itself,(but should be done from repo in another github account),(forking keeps a sync of repo, i.e if changes are made in orgin repo, it can be reflected in forked repo). 
34. Lets say i made some changes in my files, and for some reasons i dont want to commit and want to keep these changes aside in a git temp memory, from where i can recover those codes back, use git stash, and to recover the codes from stashing area, use git stash pop.

## REVERT CHANGES
1. To discard all the changes in the working area, we use git checkout filename or git checkout .(for all changes in all files).
2. To unstage all changes from staging area(keeps the change in working area), we use git reset HEAD filename or git reset HEAD * (for all)
3. To remove files from local repository,first use git log to check all the commits made, then -> use git reset HEAD~1 (it undos last 1 commit, but keeps the changes in the working directory), and if we do git reset HEAD~1 (it undos last 3 commit).
  * git reset --mixed HEAD~1 :  mixed reset(deafult reset), which removes commit and keep the changes in working directory.
  * git reset --soft HEAD~1 :  soft reset, removes commit and keep the changes in staging area.
  * git reset --hard HEAD~1 :  hard reset, removes commit as well as the changes from working directory.
4. But if the commit is made and pushed to remote repo, then git revert commitIDFromGitLog, to revert the changes from local as well as repo, but with new commit.

[To read more!](https://www.javatpoint.com/git)

