# ${{\color{red}GIT \NOTE\ }}$
# GIT NOTE
![Git Indexing](https://static.javatpoint.com/tutorial/git/images/git-index.png)
1. create a folder, and in the path of the folder, just enter cmd and click, it opens the terminal with the path of the folder.
2. Then in terminal, enter **code .**, it opens the project in vs code.
3. git init - to initialize a git repositoty in the project.
4. first project is in working directory -> git add -> goes to staging area -> git commit -> repositoty
5. git status - gives information whether any files are added or not added in staging area and also commited or not.
6. if a folder contains index.html file, then "git add index.html" adds index.html to the staging area.
7. git commit -m "any message regarding changes made", pushes from staging area to repository.
8. to add all newly added files or changes: git add .(but if any files are deleted, it wont update in repo)
9. to overcome "git add ." issue we have git add -A, it performs all changes even deletion too.
10. to undo the mistakes made in a file, lets say in index.html,we can use "git checkout index.html"
11. "git diff", to see all the changes made with respect to commited code.
12. "git diff index.html" only shows the changes made in index.html file.
13. "; wq" to get out of the git editor.
14. "git diff --staged", to see the changes in staging area.
15. "git diff HEAD", to see the changes in commit area.
16. "git log", contains entire info or history of all the commits made(contains author name, date when commit made, commit message).
17. "git log -p -n", where n means last n(numeric value) commits.
18. "git rm index.html", deletes index.html file.
19. "git rm --cached index.html", reverts index.html from staging area to working directory.
20. "git branch --list", lists all the branches.
21. "git branch branch-name" to create a new branch from the current branch.
22. "git checkout branch-name" to jump to newly created branch branch-name.
23. changes made in one branch wont be visible in its previous branches, if not merged.
24. git branch -d branch-name to delete a branch.
25. "git merge branch-name" to merge a branch with branch-name in the current branch.
26. "git checkout -b branch-name", to create and checkout branch at the same time.
27. "git commit -a -m "message"", to add and commit at the same time.
28. "git branch -M branch-name", to rename the branch name.
29. "git push -u origin branch-name", to push in the specified branch.
30. "git push -u -f origin branch-main", for force push.
31. "git remote add origin github-repo-remote-URL", to add the path of remote repository in github.
32. "git clone github-repo-remote-URL", to clone or copy the entire project from main branch of github to the path of the folder specified in bash.
[To read more!](https://www.javatpoint.com/git)

