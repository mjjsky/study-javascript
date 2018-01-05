安装git
git config --global user.name "mjjsky"
git config --global user.email "mjjsky@163.com"

--创建项目库
mkdir project-name
pwd /d/code/project-name
git init

git add readme.txt 
git commit -m "created readme.txt"

git log
git log --pretty=oneline
git reset --hard HEAD^

--查看文件命令
cat readme.txt
--撤销暂存区
git checkout -- readme.txt 

--删除文件
rm test.txt
git rm test.txt
git commit -m "remove test.txt"
--恢复删除的文件
git checkout -- test.txt
--主目录创建sshKey
ssh-keygen -t rsa -C "mjjsky@163.com"
--在主目录下生成rsa.pub 拷贝到github->ssh->ssh keys

--将本地文件添加到远程文件
git remote add project-name https://github.com/mjjsky/project-name.git
git push -u project-name master

--克隆远程库
git clone https://github.com/mjjsky/project-name.git
--新建分支并切换
## git checkout -b dev
--等同于
$ git branch dev
$ git checkout dev





