# GitHub 自动上传代码配置指南

为了配置自动上传代码到 GitHub，你需要提供以下信息：

1. **GitHub 个人访问令牌 (Personal Access Token)**
   - 访问 GitHub 设置页面：https://github.com/settings/tokens
   - 点击 "Generate new token (classic)"
   - 勾选以下权限：
     - `repo` (完整的仓库访问权限)
     - `workflow` (如果需要使用 GitHub Actions)
   - 生成并保存令牌（注意：令牌只显示一次）

2. **GitHub 仓库信息**
   - 仓库名称
   - 仓库可见性（公开/私有）
   - 仓库描述（可选）

3. **Git 本地配置**
   - Git 用户名
   - Git 邮箱地址

## 设置步骤

1. 初始化 Git 仓库：
```bash
git init
```

2. 配置 Git 用户信息：
```bash
git config user.name "你的GitHub用户名"
git config user.email "你的邮箱地址"
```

3. 添加远程仓库：
```bash
git remote add origin https://github.com/用户名/仓库名.git
```

4. 配置个人访问令牌（PAT）：
   - Windows：
   ```bash
   git config --global credential.helper wincred
   ```
   - 首次推送时输入用户名和个人访问令牌（作为密码）

5. 提交和推送代码：
```bash
git add .
git commit -m "Initial commit"
git push -u origin main
```

提供这些信息后，我可以帮助你配置自动上传代码的环境。