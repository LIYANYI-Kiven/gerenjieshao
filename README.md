# 我的个人介绍网站

这是一个基于 Jekyll 的简洁个人介绍网站模板，专为 GitHub Pages 设计。你可以通过简单的文件添加和删除来管理网站内容。

## 🚀 快速开始（部署到 GitHub）

1.  **创建仓库**：
    *   登录你的 GitHub 账号。
    *   创建一个新的仓库（Repository），命名为 `yourusername.github.io`（将 `yourusername` 替换为你的 GitHub 用户名）。
    *   *注意：如果不想用这个特定名字，也可以用任意名字，但访问地址会变成 `yourusername.github.io/repo-name`，并且需要修改 `_config.yml` 中的 `baseurl`。*

2.  **上传文件**：
    *   将本项目文件夹中的所有文件上传到你刚创建的 GitHub 仓库中。
    *   你可以使用 Git 命令行，或者直接在 GitHub 网页上点击 "Upload files"。

3.  **开启 GitHub Pages**（如果使用了 `yourusername.github.io` 命名，通常会自动开启）：
    *   进入仓库的 **Settings** (设置) -> **Pages** (页面)。
    *   在 **Build and deployment** 下，Source 选择 **Deploy from a branch**。
    *   Branch 选择 **main** (或 master) -> **/(root)**，点击 **Save**。

4.  **访问网站**：
    *   等待几分钟（GitHub Actions 构建完成后），你的网站就会在 `https://yourusername.github.io` 上线了！

## 📝 如何增加/管理内容

### 添加博客文章
1.  在 `_posts` 文件夹中创建一个新文件。
2.  文件名必须遵循格式：`YYYY-MM-DD-你的标题.md`（例如 `2025-12-26-my-diary.md`）。
3.  文件内容头部必须包含以下信息：
    ```yaml
    ---
    layout: post
    title:  "这里写文章标题"
    date:   2025-12-26 12:00:00 +0800
    ---
    ```
4.  在下方使用 Markdown 格式写正文。
5.  **提交更改到 GitHub**，网站会自动更新。

### 修改个人信息
*   打开 `_config.yml` 文件，修改 `title`（网站标题）、`description`（描述）、`email` 等信息。
*   打开 `about.md` 文件，修改“关于我”页面的内容。

### 修改首页欢迎语
*   打开 `index.html`，找到 `<div class="hero">` 部分进行修改。

## 🎨 本地预览（可选）
如果你想在本地电脑上预览：
1.  安装 Ruby 和 Jekyll。
2.  在终端运行 `bundle install`。
3.  运行 `bundle exec jekyll serve`。
4.  访问 `http://localhost:4000`。
*（对于普通用户，建议直接在 GitHub 上修改和预览）*
