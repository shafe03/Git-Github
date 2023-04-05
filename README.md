
### Git advance

1. Git diff commitsid HEAD 
2. Git difftool commitid HEAD
3. Git help diff
4. Fast forward merge, automatic merge, manual merge
5. Git checkout -b branchNameWeWannaCreate
6. Git branch
7. Git checkout master
8. Git update
9. Git checkout -b very-bad
10. Git mergetool
11. Light weight tag, annotations tag
12. Git tag mytag
13. Git tag --list
14. Git tag -d mytag
15. Git tag -a v1.0 -m "Released V1.0"
16. Git show v1.0
17. Git stash
18. Git stash list
19. Git stash pop
20. Reset-----soft----
21. Git reset commitId --soft
22. Git reset commitId --mixed
23. Git reset commitId --hard
24. Git reflog
25. Git reset --hard commitID (to back to that commit point, this commit id is taken from git reflog)



### GITHUB

1. Git remote -v
2. Git remote add origin githupRepositoryHttps/sshLink
3. Git push -u origin master --tags (to push local      repository to remote repository, -u indicate tracking between local and remote repository)




### ssh authentication

1. git push origin master
2. ssh-keygen -t rsa -C "yourEmail@address" (-t =type, here type is rsa, -C for common name)
3. npp id_rsa.pub (copy all text from here and paste it to github ssh key)
4. ssh -T git@github.com (to confirm machine can communicate through ssh key with github)
5. Id_rsa, id_rsa.pub



### GITHUB REPOSITORY

1. Git clone githubRepositoryAddress (here repository name is my-website)
2. rm -rf my-website (to remove repository whole folder from local repository)
3. Git clone githubRepositoryAddress website (to change the repository name in local machine)
4. Git push
5. Git config --global push.default simple
6. Git fetch
7. Git pull
8. Git push
9. Git remote set-url origin repositoryAddress (if change name of repository in hithub)
10. Git remote show origin
11. Git show commitID (this commit id is copy from github )



### GITHUB REPOSITORY BRANCH

1. Git checkout -b remove-lipsum
2. Git push -u origin remove-lipsum (-u means traking relation, here remote is origin, and tracking branch remove-lipsum, this command will also create a new branch on github)
3. Git merge
4. Git branch -d remove-lipsum (-d = delete)
5. Gir branch -a
6. Git fetch -p (-p is a prune option it will look for any dead branches and will remove its reference)
7. Git checkout update-readme (this repository is not in local repo ita on github but this command will create local repo of update-readme )
8. Git pull --all
9. Git merge update-readme
10. Git push origin :update-readme (this command will delete github branches feom command line)
11. Git pull --rebase (local cimmit will be 1 commit ahead of remote head)



### Tags

1. Git tag unstable develop
2. Git tag stable main
3. Git tag -a v1.0-alpha -m "Release v1.0" commitID
4. Git show (with annotations tag)
5. Git tag
6. Git tag -a v2.0-alpha -m "Release v2.0" commitsid
7. Git push origin stable (to push a single tag)
8. Git push --tag ( to push all tags)
9. Git fetch -p
10. Git tag -d v1.0-alpha
11. Git push origin :v2.0-alpha (to delete remote tags)
12. Git tag -f unstable commitID (to assign tag to specific commit id )
13. Git push --force origin unstable
14. Git pull (github creat light weight tag)


### COMARING DIFFERENCES

1. Develop@{3days}
2. Master@{2020-05-15}
3. HEAD@{3}
4. HEAD^ (HEAD MINUS ONE)


1. Git remote add upstream githubaddresslinkofforkingrepoaddress
2. Git pull upstream feature-readme
3. Gir push origin main
