# git command Project for github testing

# crate github repository

touch README.md 

git init 

git add README.md 

git commit -m “first commit” 

git remote add origin https://github.com/HairanWu/gitcommand.git

git push -u origin master

# create tag
git branch

git tag

git tag -a v0.1 -m "version 0.1 released"

git show v0.1

git push origin v1.0

git push origin --tags

git tag -d v0.1

# create branch

git checkout -b dev

git branch dev

git checkout dev
