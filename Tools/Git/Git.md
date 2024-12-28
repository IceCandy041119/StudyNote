# GitNotes  

## 目录

- [基础命令](#基础命令)
- [查看日志命令](#查看日志命令)
- [分支和合并](#分支和合并)
- [远端操作](#远端操作)
- [撤销](#撤销)
- [高级操作](#高级操作)

## 基础命令  

- `git config --global user.name <username>` 刚安装时使用，进行用户签名  
- `git config --global user.email <useremail>` 刚安装时使用，进行用户签名  
- `git init` 初始化本地仓库   
- `git status` 查看本地库状态  
- `git add <filename>` 添加到暂存区  
- `git commit <filename>` 提交到本地库
- `git help <command>` 获取git命令的帮助信息
- `git diff <filename>` 显示与暂存区文件的差异  
- `git diff <revision> <filename>` 显示某个文件两个版本之间的差异  

## 查看日志命令

- `git log` 显示历史日志  
  - `git log --all --graph --decorate` 可视化历史记录（有向无环图）  
- `git reflog` 查看reflog信息
   
>**`log` 与 `reflog` 的区别**  
>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`log` 显示当前HEAD及其祖先。也就是说，它会打印HEAD指向的提交，然后是其父级、其父级的父级...。它会通过递归查找每个提交的父级来遍历存储库的祖先。`reflog` 不会遍历HEAD的祖先，它是HEAD指向的提交的有序列表，是存储库的撤销历史记录，它不是存储库本身的一部分（它与提交本身分开存储），也不包含在推送，提取或克隆中，它纯粹是本地的。  
>另外：了解 `reflog` 意味着一旦提交，就不会真正丢失在存储库里的数据。如果不小心重置为较旧的版本，或错误的重新设置了基数，或任何其他直观地“删除”操作，都可以使用 `reflog` 查看之前的位置，然后通过 `git reset --hard <hashkey>` 返回该引用以恢复之前的状态。引用不止意味着提交，也意味着背后整个的历史记录，但reflog条目并不会永久保留，但错误至少在两周内会是安全的  

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
>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;前者只去更新HEAD指针，列如，在使用时，从主线切换到其他地方，只有HEAD指针去移动，而后者，则将主线指针也一并带了过来，为此可能会出现丢失数据的情况，就要用到 `reflog` 了  

## 远端操作  

- `git remote` 列出远端  
- `git remote add <name> <url>` 添加一个远端  
- `git push <remote> <local branch>:<remote branch>` 将对象传送至远端并更新远端引用  
- `git branch --set-upstream-to <remote>/<remote branch>` 创建本地和远端分支的关联关系  
- `git fetch` 从远端获取对象/索引  
- `git pull` 相当于git fetch;git merge  
- `git clone <url>` 从远端下载仓库  

## 撤销

- `git commit --amend` 编辑提交的内容或信息  
- `git reset HEAD <filename>` 恢复暂存文件  
- `git checkout -- <filename>` 丢弃修改  
- `git restore` git2.32 版本后取代 git reset 进行许多撤销操作

>**`checkout -- <filename>` 与 `reset HEAD <filename>` 区别**  
>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;前者如果文件没有添加到缓存区，那么将最近一次提交的版本替换工作目录中的文件，丢弃本地的修改，后者仅将文件从暂存区中移除

## 高级操作  

- `git config` Git 是一个高度可定制的工具  
- `git clone --depth=1` 浅克隆(shallow clone)，不包括完整的版本历史信息  
- `git add -p` 交互式暂存  
- `git rebase -i` 交互式变基  
- `git blame` 查看最后修改某行的人  
- `git stash` 暂时移除工作目录下的修改内容  
- `git bisect` 通过二分查找搜索历史记录  
- `.gitignore` 指定故意不追踪的文件(不是命令，是dot file)  

