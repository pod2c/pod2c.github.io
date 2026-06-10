# PhD Homepage Template for GitHub Pages

这是一个可以直接部署到 GitHub Pages 的 PhD 个人主页模板。

## 你需要改哪些地方

主要修改 `index.html`：111

- `Your Name`
- `Department`
- `University`
- `Prof. Advisor Name`
- `Research Area 1 / 2 / 3`
- `your.email@university.edu`
- Google Scholar / GitHub / LinkedIn 链接
- Publications 部分的论文标题、作者、链接和 BibTeX
- News / Teaching / Service / Awards

头像：

- 把你的照片放到 `assets/` 文件夹，例如 `assets/profile.jpg`
- 然后把 `index.html` 里的这一行：

```html
<img class="portrait" src="assets/avatar.svg" alt="Portrait of Your Name" />
```

改成：

```html
<img class="portrait" src="assets/profile.jpg" alt="Portrait of Your Name" />
```

CV：

- 把你的 CV PDF 放到 `files/` 文件夹
- 文件名改成 `cv.pdf`
- 页面里的 CV 按钮会自动指向 `files/cv.pdf`

## 最简单的 GitHub Pages 上线方式

1. 在 GitHub 新建一个仓库，仓库名必须是：

```text
your-github-username.github.io
```

例如你的 GitHub 用户名是 `alicewang`，仓库名就是：

```text
alicewang.github.io
```

2. 把这个模板里的所有文件上传到仓库根目录。注意是上传 `index.html`、`assets/`、`files/` 这些内容，不是把整个 `phd-homepage-github-pages` 文件夹套进去。

3. 进入仓库的：

```text
Settings → Pages
```

4. 在 `Build and deployment` 里选择：

```text
Source: Deploy from a branch
Branch: main
Folder: / (root)
```

5. 保存后访问：

```text
https://your-github-username.github.io/
```

GitHub Pages 发布后可能需要等一小段时间才会显示。

## 本地预览

你可以直接双击 `index.html` 打开，也可以在这个文件夹里运行：

```bash
python3 -m http.server 8000
```

然后打开：

```text
http://localhost:8000
```

## 官方参考

- GitHub Pages Quickstart: https://docs.github.com/pages/quickstart
- Configuring a publishing source: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
