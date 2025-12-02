## Initiate git
1. mkdir dirname
2. cd dirname
3. git init
4. ls -la .git
5. touch filename

## Link remote repo
1. Create repo in Github
2. git remote add origin url
3. git remote -v (for checking)
4. git push origin branchname
5. git remote rm origin
6. rm -rf .git*
7. git fetch origin branchname

## Standard git
- git add filename
- git add *
- git reset *#reverses the git add command*
- git commit -m 'message'
- git branch branchname
- git checkout branchname
- git status
- git log
- git branch ( , -a, -r)
- git merge branchname
- git push origin branchname (--force)
- git branch -d branchname
- git checkout -b branchname
- git checkout -b localbranch  origin/remotebranch
- git stash (-k)
- git branch -m newname
- git clone url newname
- git reflog
- git tag \<tagname\>
- git push origin \<tagname\>
- git push origin --tags
- git tag
- git tag -d \<tagname\>
- git push --delete origin \<tagname\>
- git push origin --delete branchname
- git branch -vv
- git branch --set-upstream-to=origin/branchname branchname
- git push -u origin branchname

## Large files
- cd dirname
- git lfs install
- git lfs track '*filename.ext'
- git add .gitattributes
- git lfs migrate import --include='*file.ext'
- git actions as usual

# Git synchronisation
## 1. Verify branches status
- git status
- git branch
- git branch -r
## 2. Check sync status
- git branch -vv
- git checkout branchname
- git branch --set-upstream-to=origin/branchname branchname
- git branch -vv
- git push origin branchname
- git pull
## 3. Check dev and master are on the same commit
- git checkou branch1
- git log branch2..branch1
- git checkout branch2
- git log branch1..branch2



















