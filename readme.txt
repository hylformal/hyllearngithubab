git is a version control system.
git is free software.
hyl@hyl:~/hylgit$ git add readme.txt //第一步，加入文件，可以一次加入多个文件
hyl@hyl:~/hylgit$ git commit -m "wrote a readme file"//第二步，提交并说明
git status //查看状态
git diff //查看差异,git diff HEAD -- readme.txt,查看版本库与工作区文件的差异
hyl@hyl:~/hylgit$ git log --pretty=oneline//查看修改日志
git reset --hard commit_id或者HEAD^(前一次)HEAD~100(前100次)，HEAD指向版本
git log//穿梭前，查看提交历史，以便确定要回退到哪个版本
git reflog//要重返未来，查看命令历史，以便确定要回到未来的哪个版本
场景1：git checkout -- readme.txt//直接丢弃工作区的修改
场景2：git reset HEAD readme.txt//丢弃暂存区修改，回到场景1
