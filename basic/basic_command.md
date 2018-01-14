# 基本命令
* setting， 所有的配置放在<HOME>/.gitconfig
```
git config --global user.email "xxxx@qq.com"
git config --global user.name "hellozhaojian"
git config --global credential.helper store
git config --list #  查看
```
* checkout
```
git clone https://github.com/hellozhaojian/github.git
```
* 查看状态
```
git status
```
* 比较
```
git diff
```
* 添加
```
command git add [file or dir]
```

* 查看git的远程指代关系
```
git remote -v 
我们发现
origin https://github.com/user2/repository.git (fetch)
origin https://github.com/user2/repository.git (push)
本地关于远程仓库的指代是origin
```
* 提交
```
vi .git/config 修改origin下面的url，类似https://user@....
git commit -m 'xxx'
git push https://github.com/hellozhaojian/github master
OR
git push orign master
```

* 新建branches
```
1. 查看有哪些branch
   git branch [-a | -r]
     -a 所有
     -r 远程
     默认是本地的
2. 切换到一个branch中
   git checkout <branch_name>

```

* merge
```
1. git merge <other_branch_name>
   记住这里的branch是本地的branch
``` 
