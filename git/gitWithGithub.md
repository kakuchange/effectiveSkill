# install git
https://git-scm.com/downloads


# config
git config --global user.name kaku
git config --global user.email scugjs@163.com


# initial example
git init
git status

git add/git commit -m 
git diff readme.md

git log
git log --pretty=oneline

git reset --hard HEAD^
git reset --hard HEAD~100

git reflog

git reset --hard 6fcfc89

cat readme.md

git checkout -- file
^git checkout -- readme.md$ mean remove workSpace change 回到暂存区或库中版本！


# push to github
C:\Users\\****\\.ssh  
id_rsa.pub  
github.com/kakuchange/settings  
add SSH keys
local repository sync with github repository
# push local master 
git push -u origin master #first push
git push origin master


# command example
git checkout -b dev #创建并切换 相当于 git branch dev + git checkout dev
git branch #查看当前分支
git branch -D dev
git stash #隐藏工作状态
git stash apply & git stash drop


# 各种取消操作
git rm –cached filename#add之后取消！
git command --amend #重新编辑提交message！合并提交！
git checkout -- readme.md #撤销本地修改

### 1.commit后修改回到某个ish位置，连同硬盘（本地修改）
git reset --hard <commit_ish>  
### 2.修改HEAD，提交记录变，但文件不变（本地未修改）默认！
git reset --mixed <commit_ish>  
### 3.soft相当于mixed方法后再git add
git reset --soft <commit_ish>  

