# MyCSNotes
个人计算机学习笔记
Personal Computer Science Learning Notes

- Bash Command Complete:
	个人GNU Bash 命令大全和用户手册。
	Personal GNU Bash command complete and user guide.
  
- Learn C++ Tutorial - Learning Note:
	在线教程[Learn C++ – Skill up with our free tutorials](https://www.learncpp.com/)的学习笔记——我最喜欢的C++教程。
	Learning Note on on-line tutorial [Learn C++ – Skill up with our free tutorials](https://www.learncpp.com/), which is my favorite C++ tutorial.
## Git guide for commit & push

### On Unix-like

Take Ubuntu, for example:

```bash
cd localRespositoryDirectory/
git init  #Create .git folder in current directory
#Recommendatory, add ssh github address as remote. Make sure that SSH is configured before push (see following)
git remote add origin git@github.com:githubAccountName/repositoryName.git
#Unrecommendatory, add https github address as remote
git remote add origin https://github.com/githubAccountName/repositoryName.git

git add filename.md
git config --global user.email "your-email@example.com"
git config --global user.name "Your Name"
#Or local config
git config user.email "your-email@example.com"
git config user.name "Your Name"
git commit -m "message of commit"
git branch -M master
git push -u origin master  #Set upstream at first time
git branch --set-upstream-to=origin/master master  #Above do this incidentally
git push  #Use this after above
```

#### Local SSH key genarating & GitHub config

```bash
ssh-keygen -t rsa -b 4096 -C "your-email@example.com"
cat ~/.ssh/id_rsa.pub  #SSH key her
#copy this output
```

GitHub home -> account (right top) -> settings -> SSH and GPG kys -> New SSH key

一定要复制全部的`id_rsa.pub`内容，即从`ssh-rsa`到最后。
Must copy the all content in `id_rsa.pub`, i. e. from `ssh-rsa` to the end.



