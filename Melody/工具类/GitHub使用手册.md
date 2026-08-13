## 首次上传完整命令

```
# 1. 进入你的文件夹（如果终端已经在该文件夹可跳过）
cd /path/to/你的文件夹

# 2. 初始化本地 Git 仓库
git init

# 3. 把所有文件加入暂存区
git add .

# 4. 提交到本地仓库，-m 后面是说明，随便写
git commit -m "first commit"

# 5. 把本地分支改名为 main（GitHub 现在默认叫 main）
git branch -M main

# 6. 关联 GitHub 上的仓库，把网址换成你自己的
git remote add origin [](@replace=10001)你的用户名/你的仓库名.git

# 7. 推送到 GitHub（-u 表示以后直接 git push 就行）
git push -u origin main
```

## 修改后上传文件的命令
在你电脑上**修改完文件后**，只需要走标准的“三步走”把改动同步到 GitHub 就行（前提是你之前已经 `git init` + `git remote add origin ...` + 首次 `git push -u origin main` 做过了）：

```
# 1. 把你改过的、新增的文件加入暂存区
git add .

# 2. 提交到本地仓库，-m 后面写这次改了啥
git commit -m "更新了xxx文件"

# 3. 推到 GitHub（首次推过之后，直接 git push 就行）
git push
```