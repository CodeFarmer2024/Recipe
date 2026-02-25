# Recipe Book

这个仓库的文档可以直接生成电子书（EPUB/PDF）和静态站点，并自动发布到 GitHub Pages。

## 电子书下载

- EPUB：[/ebooks/recipe.epub](/ebooks/recipe.epub)
- PDF：[/ebooks/recipe.pdf](/ebooks/recipe.pdf)

发布到 GitHub Pages 后，上述路径会在站点根目录下可直接访问。

## 本地构建

1. 安装依赖

```sh
npm install
```

2. 生成静态站点 + 电子书

```sh
npm run build
```

输出目录：
- 静态站点：`_book/`
- 电子书：`_book/ebooks/recipe.epub`、`_book/ebooks/recipe.pdf`

## 仅生成静态站点

```sh
npm run build:site
```

## 仅生成电子书

```sh
npm run build:epub
npm run build:pdf
```

## 依赖说明

生成 EPUB/PDF 需要系统安装 Calibre（提供 `ebook-convert` 命令）。
另外请确保系统安装了 CJK 字体（如 Noto CJK），否则 PDF/EPUB 可能出现乱码。
