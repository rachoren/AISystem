添加一个新的远程指向原始仓库（upstream repository）。
- git remote add upstream git@github.com:chenzomi12/AISystem.git

验证远程仓库是否已成功添加。
- git remote -v 

设置你的本地分支跟踪远程分支。假设你想要跟踪main
- git branch --set-upstream-to=upstream/main main

完成这些步骤后，你的本地分支将会自动推送到你的fork，同时保持与原始仓库同步。当你需要获取原始仓库的更新时，可以使用git fetch upstream，然后可以选择合并到你的分支中，或者rebase你的分支。
- git fetch upstream
- git checkout main
- git merge upstream/main
