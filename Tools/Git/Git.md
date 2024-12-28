# GitNotes  

## 目录

- [基础命令](#基础命令)
- [查看日志命令](#查看日志命令)
- [分支和合并](#分支和合并)

## 基础命令  

- `git config --global user.name <username>` 刚安装时使用，进行用户签名  
- `git config --global user.email <useremail>` 刚安装时使用，进行用户签名  
- `git init` 初始化本地仓库   
- `git status` 查看本地库状态  
- `git add <filename>` 添加到暂存区  
- `git commit <filename>` 提交到本地库
- `git help <command>` 获取git命令的帮助信息  

## 查看日志命令

- `git log` 显示历史日志  
  - `git log --all --graph --decorate` 可视化历史记录（有向无环图）  
- `git reflog` 查看reflog信息
   
>**`log` 与 `reflog` 的区别**  
>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**`log` 显示当前HEAD及其祖先。也就是说，它会打印HEAD指向的提交，然后是其父级、其父级的父级...。它会通过递归查找每个提交的父级来遍历存储库的祖先。`reflog` 不会遍历HEAD的祖先，它是HEAD指向的提交的有序列表，是存储库的撤销历史记录，它不是存储库本身的一部分（它与提交本身分开存储），也不包含在推送，提取或克隆中，它纯粹是本地的。
>另外：了解 `reflog` 意味着一旦提交，就不会真正丢失在存储库里的数据。如果不小心重置为较旧的版本，或错误的重新设置了基数，或任何其他直观地“删除”操作，都可以使用 `reflog` 查看之前的位置，然后通过 `git reset --hard <hashkey>` 返回该引用以恢复之前的状态。引用不止意味着提交，也意味着背后整个的历史记录，但reflog条目并不会永久保留，但错误至少在两周内会是安全的**

## 分支和合并

- `git branch` 显示分支  
- `git branch <name>` 创建分支  
- `git merge <revision>` 合并到当前分支  
- `git mergetool` 使用工具来处理冲突  
- `git rebase` 将一系列补丁变基为新的基线  
- `git checkout <revision>` 更新HEAD和目前的分支  
  - `git checkout -b <name>` 创建并切换分支
- `git reset --hard <revision>` 重置HEAD指针到指定的提交

>**`checkout` 与 `reset --hard` 的区别**  
>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**前者只去更新HEAD指针，列如，在使用时，从主线切换到其他地方，只有HEAD指针去移动，而后者，则将主线指针也一并带了过来，为此可能会出现丢失数据的情况，就要用到 `reflog` 了**  


