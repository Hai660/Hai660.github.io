# 将仓库重命名为 Hai660.github.io

按照以下步骤将仓库重命名为与 GitHub 用户名相同的名称，这样网站就可以在根路径运行。

## 步骤 1：在 GitHub 上重命名仓库

1. 访问你的仓库：https://github.com/Hai660/hai
2. 点击仓库页面右上角的 **"Settings"**（设置）标签
3. 向下滚动到页面底部的 **"Danger Zone"**（危险区域）部分
4. 点击 **"Change repository name"**（更改仓库名称）
5. 将仓库名从 `hai` 改为 `Hai660.github.io`（注意：必须与你的 GitHub 用户名完全相同）
6. 点击 **"I understand, change repository name"**（我理解，更改仓库名称）

## 步骤 2：更新本地 Git 远程仓库地址

在 PowerShell 中运行以下命令：

```bash
git remote set-url origin https://github.com/Hai660/Hai660.github.io.git
git remote -v
```

验证远程仓库地址已更新。

## 步骤 3：推送代码

```bash
git push
```

## 步骤 4：更新 GitHub Pages 设置

1. 访问新仓库：https://github.com/Hai660/Hai660.github.io
2. 点击 **"Settings"** → **"Pages"**
3. 确认设置：
   - Source: **Deploy from a branch**
   - Branch: **main**
   - Folder: **/ (root)**
4. 点击 **"Save"**

## 步骤 5：访问你的网站

等待几分钟后，你的网站将在以下地址可用：

**https://Hai660.github.io**

注意：不再需要 `/hai/` 子路径了！

## 重要提示

- 仓库名必须与 GitHub 用户名**完全相同**（大小写敏感）
- GitHub Pages 会自动将 `用户名.github.io` 仓库部署到根路径
- 如果之前有其他仓库也叫 `Hai660.github.io`，需要先删除或重命名它
- 域名生效可能需要几分钟时间

