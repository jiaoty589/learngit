1.配置用户名、邮箱
git config --global user.name 'Your Name'.
git config -- global user.email 'Email'.
--global   这台机器的所有Git仓库都会使用这个配置。

查看用户名、邮箱
git config user.name.
gif config user.email.


2.初始化git仓库
将当前目录变为git可以管理的仓库
git init
Git会自动创建一个master分支。


3.将文件添加到仓库
（1）git add
将文件添加到暂存区（Stage）
git add file
（2）git commit 
git commit -m 'message'
将暂存区的所有内容提交到当前分支。

简单理解为，需要提交的文件通通放到暂存区，然后，一次性提交暂存区的所有修改。


4.查看仓库状态
git status  
查看哪些文件被修改了

5.查看文件修改内容
git diff 
git diff file


6.查看历史
git log
显示最近到最远的提交日志，如果输出信息太多，可以加上  --pretty=oneline
git log --pretty=oneline


7.回退版本
git reset
在git中，HEAE代表当前版本，HEAD^代表上个版本，HEAD^^代表上上的版本。（上100个版本，HEAD~100）
gir reset --hard HEAD^


8.工作区和暂存区
初始化的目录就是一个工作区。
.git是Git的版本库。
