# hugo github 个人 blog

## 安装 hugo

```bash
hugo is the main command, used to build your Hugo site.

Hugo is a Fast and Flexible Static Site Generator
built with love by spf13 and friends in Go.

Complete documentation is available at https://gohugo.io/.

Usage:
  hugo [flags]
  hugo [command]

Available Commands:
  completion  Generate the autocompletion script for the specified shell
  config      Print the site configuration
  convert     Convert your content to different formats
  deploy      Deploy your site to a Cloud provider.
  env         Print Hugo version and environment info
  gen         A collection of several useful generators.
  help        Help about any command
  import      Import your site from others.
  list        Listing out various types of content
  mod         Various Hugo Modules helpers.
  new         Create new content for your site
  server      A high performance webserver
  version     Print Hugo version and environment info
```

## hugo 目录结构

```bash
so@Sos-MacBook-Pro Socool % tree
.
├── archetypes
│   └── default.md
├── assets
├── content
├── data
├── hugo.toml
├── i18n
├── layouts
├── static
└── themes
```

## 设置 hugo 创建网站新项目
```bash
so@Sos-MacBook-Pro ~ % hugo new site Socool -f yml     

Congratulations! Your new Hugo site was created in /Users/so/Socool.

Just a few more steps...

1. Change the current directory to /Users/so/Socool.
2. Create or install a theme:
   - Create a new theme with the command "hugo new theme <THEMENAME>"
   - Install a theme from https://themes.gohugo.io/
3. Edit hugo.toml, setting the "theme" property to the theme name.
4. Create new content with the command "hugo new content <SECTIONNAME>/<FILENAME>.<FORMAT>".
5. Start the embedded web server with the command "hugo server --buildDrafts".

See documentation at https://gohugo.io/.
```

## 发布一篇新文章

```bash
so@Sos-MacBook-Pro Socool % hugo new docs/test.md
Content "/Users/so/Socool/content/docs/test.md" created
```

## 安装主题 PaperMod

- 初始化 git

```bash
git init
Initialized empty Git repository in /Users/so/Socool/.git/
```
- 克隆主题仓库

```bash
so@Sos-MacBook-Pro Socool % git clone https://github.com/adityatelange/hugo-PaperMod themes/PaperMod --depth=1
Cloning into 'themes/PaperMod'...
remote: Enumerating objects: 134, done.
remote: Counting objects: 100% (134/134), done.
remote: Compressing objects: 100% (115/115), done.
remote: Total 134 (delta 34), reused 58 (delta 15), pack-reused 0
Receiving objects: 100% (134/134), 232.65 KiB | 2.47 MiB/s, done.
Resolving deltas: 100% (34/34), done.
```
- 添加主题模块

```bash
so@Sos-MacBook-Pro Socool % git submodule add --depth=1 https://github.com/adityatelange/hugo-PaperMod.git themes/PaperMod
Adding existing repo at 'themes/PaperMod' to the index
```
