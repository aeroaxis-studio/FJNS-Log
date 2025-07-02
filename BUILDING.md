# 构建与更新

该项目使用 [GitBook](https://github.com/GitbookIO/gitbook) 生成文档站点。

## 环境
1. 安装 Node.js 14 或更新版本
2. 全局安装 gitbook-cli：
   ```bash
   npm install -g gitbook-cli
   ```

## 安装依赖
在项目根目录执行：
```bash
npm install
```
这会安装 package.json 中设定的依赖。

## 本地预览
```bash
npm run serve
```
打开 http://localhost:4000 即可预览。

## 构建
直接生成静态文件：
```bash
npm run build
```
构建结果会保存在 `_book/` 目录。

## 更新文档
1. 编辑 Markdown 文件，并在 `SUMMARY.md` 中列出新文件
2. 重新执行 `npm run build` 生成新文档
