git is distributed version control system.
git is free software.
git add readme.txt 添加文件到git大门口
git add readme1.txt readme2.txt 添加多个文件到git大门口
git add ./ 把文件下所有的文件添加到git大门口
git commit -m "添加了什么内容" 提交文件到git仓库，冒号里面是每次修改了什么的提示
git commit --all -m "一次性添加所有文件到git仓库"  不需要输入git add就可以一次性添加所有文件到git仓库
git status 查看文件有没有被修改过
git diff readme.txt 查看修改的内容
git log 查看提交历史记录（如果嫌输出信息太多，看得眼花缭乱的，可以试试加上--pretty=oneline参数：）
例 $ git log --pretty=oneline
git reflog 查看命令历史记录
HEAD 指向的版本就是当前版本，因此，Git允许我们在版本的历史之间穿梭，使用命令git reset --hard commit_id
$ git checkout -- test.txt 恢复
git rm text.txt 删除