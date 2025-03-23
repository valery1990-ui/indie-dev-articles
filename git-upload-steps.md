# Git命令上传代码步骤说明

每个命令执行后，等待我的确认再继续下一步。

## 步骤1：检查当前状态
```bash
git status
```

## 步骤2：添加所有文件
```bash
git add .
```

## 步骤3：确认文件已暂存
```bash
git status
```

## 步骤4：创建提交
```bash
git commit -m "Initial commit"
```

## 步骤5：检查远程仓库配置
```bash
git remote -v
```

## 步骤6：添加远程仓库（如果还没添加）
```bash
git remote add origin https://github.com/valery1990-ui/indie-dev-articles.git
```

## 步骤7：推送代码
```bash
git push -u origin master
```

让我们从第一步开始，执行 `git status` 来检查当前状态。