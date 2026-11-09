# 我的个人园地 · 使用说明（零基础）

这个文件夹是一个可以直接发布到 GitHub Pages 的个人网站模板。
里面的示例文字和照片都是占位内容，公开使用之前请替换成自己的。

## 1. 第一次发布

1. 注册 GitHub：https://github.com/
2. 点击右上角 `+` → `New repository`。仓库名必须是 `你的GitHub用户名.github.io`，例如 `xiaoming.github.io`。
3. 选择 `Public`，点击 `Create repository`。
4. 在新仓库选择 `uploading an existing file`，或 `Add file` → `Upload files`。
5. **先解压 ZIP 文件**；把这个文件夹内部的所有内容（`index.html`、其他 html、`assets`、`articles`、`images` 等）拖入上传区。不要只上传 zip；也不要把最外层的 personal-website-starter 文件夹再嵌套一层。
6. 点击 `Commit changes`，确认保存到 `main` 分支。
7. 打开 `Settings` → `Pages` → `Build and deployment` → `Source: Deploy from a branch` → `Branch: main` 和 `/ (root)` → `Save`。
8. 访问 `https://你的GitHub用户名.github.io/`，发布可能需要几分钟。

## 2. 要替换个人介绍

打开 `index.html` 或 `about.html`，点击 GitHub 的铅笔图标进行编辑。找到原来的中文介绍，替换成你的内容，点 `Commit changes` 保存。

## 3. 要发布一篇新文章

- 打开 `articles/first-note.html`，参照其内容新建 `articles/my-second-note.html`。
- 替换页面中 `<title>`、`<h1>`、`<article class="article-body">` 内的段落文字。段落请放在 `<p>……</p>` 中。
- 在 `writing.html` 的文章列表里添加一条链接，例如 `<a href="articles/my-second-note.html">新文章标题</a>`。
- 也可以在 `index.html` 的最近文章列表添加同样的链接。
- 全部保存（Commit changes）后网站会自动更新。

## 4. 替换照片

在 `images` 文件夹中上传自己的 JPG 照片，文件名为 `photo-01.jpg`、`photo-02.jpg`、`photo-03.jpg`，覆盖占位文件。
以后可以继续添加文件，再在 `photos.html` 复制一段 `<figure class="photo">……</figure>`，把文件名和说明改掉。
照片公开前请注意人物隐私、定位和版权，压缩体积更容易加载。

## 5. 视频怎样放

大视频优先上传到 B 站或 YouTube，再将页面链接或嵌入播放器代码放到 `videos.html`。
例如普通链接：`<a href="https://你的视频网址" target="_blank" rel="noopener noreferrer">观看我的视频</a>`。
如果你提供具体的 B 站或 YouTube 地址，可以让 ChatGPT 帮你写对应的播放器代码。

## 文件说明

- `index.html`：首页
- `writing.html`：文字目录
- `photos.html`：摄影页
- `videos.html`：视频页
- `about.html`：个人介绍
- `articles/first-note.html`：第一篇示例文章
- `assets/style.css`：网页样式，控制颜色、字号和布局
- `images/*.jpg`：图片

不需要安装 Python、Node.js 或其它开发环境。初期所有操作都可以直接在 GitHub 网页上进行。
