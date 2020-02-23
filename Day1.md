# Day 1
#### 创建本地Git repository
* 在Git bash 输入
```
$ git config --global user.name "Your Name"
$ git config --global user.email "Your Email"
```
* 创建一个空目录，存储Git版本库
```
$ mkdir <path/directory>
$ cd <path/directory>
$ pwd // 显示当前目录
```
* 将该目录变为Git仓库
```
$ git init
```
----
#### 文件操作
* 新建文件
```
$ vi filename.txt
```
* 在文本文件中写入内容
```
hello github.com // 版本1
```
* 将该文件添加进仓库
```
$ git add filename.txt
$ git commit -m "the description"
```
* 修改文件内容后，查看代码库的状态
```
$ git status 
```
* 修改文件内容后，查看前后两个版本的差别
```
$ git diff
```
* 提交修改过后的文件
* 文件提交记录
```
$ git log // 可以获得commit ID
$ git reflog // 若Git bash关闭后，可以查看版本操作记录，以获得commit ID
```
* 版本后退与前进
```
// 后退方法1
$ git reset --hard HEAD^ // 回退一个用^，回退多个用~number
// 后退方法2 & 前进方法1
$ git reset --hard commit ID // 若回退两个版本，前进到最新commit ID，则倒数第二个版本也会被恢复
```
