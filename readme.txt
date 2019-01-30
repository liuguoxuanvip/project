git is distributed version control system.
git is free software.
git init 创建git目录
git add readme.txt 添加文件到git大门口
git add readme1.txt readme2.txt 添加多个文件到git大门口
git add ./ 把文件下所有的文件添加到git大门口
git commit -m "添加了什么内容" 提交文件到git仓库，冒号里面是每次修改了什么的提示
git commit --all -m "一次性添加所有文件到git仓库"  不需要输入git add就可以一次性添加所有文件到git仓库
git status 查看文件有没有被修改过
git diff readme.txt 查看修改的内容
git log 查看提交历史记录（如果嫌输出信息太多，看得眼花缭乱的，可以试试加上--pretty=oneline参数：或者 git log --oneline）
例 $ git log --pretty=oneline
git reflog 查看命令历史记录
HEAD 指向的版本就是当前版本，因此，Git允许我们在版本的历史之间穿梭，
使用命令git reset --hard commit_id  （例：git reset --hard 68e82ad）
或者使用命令 git reset --hard Head~0  （Head~0代表当前版本，Head~1代表上一个版本，依次类推）
$ git checkout -- test.txt 恢复
git rm text.txt 删除
##创建分支
git branch dev
##切换分支
git checkout dev
##查看分支
git branch
##合并分支
git merge(合并) dev（自定义文件夹名） 

##提交代码到github（当做git服务器使用）
git push 【地址】 master
示例：git push https://github.com/liuguoxuanvip/project.git
会把当前分支的内容上传到远程的master分支上

git pull 【地址】 master
示例：git pull https://github.com/liuguoxuanvip/project.git
会把远程分支的数据得到：{注意本地-要初始化一个仓库！git innit} *常用

git clone 【地址】
会得到远程仓储相同的数据，如果多次执行会覆盖本地内容 *不常用


ssh-keygen -t rsa -C "123635530@qq.com" 生成公钥和私钥
