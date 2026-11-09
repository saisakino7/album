# SOUNDS OF MENGMAOLONE · SAISAKI 专辑链接页

## 文件
- `index.html`：网页本身，封面已嵌在里面
- `cover.jpg`：分享链接时的预览图（1200×900）
- `icons/`：平台图标，文件名必须是：
  `spotify.png` `netease.png` `youtube.png` `qishui.png` `applemusic.png` `qqmusic.png`
  （建议正方形，至少 102×102 像素；没放图标的平台会显示彩色圆角色块）

`cover.png` 是原图，不需要上传。

## 改内容
打开 `index.html`，搜索 `只需要改这里`：
- `LINKS` 里每个平台的 `url:""` 填上专辑链接，留空 = 显示「即将上线」
- `TELEGRAM = ""` 填群链接，例如 `https://t.me/xxx`
- `TEXT` 里改中英文简介（`statement` 是大标语，`intro` 是正文）

## 上线（GitHub Pages）
1. 注册 GitHub，新建一个公开仓库，名字叫 `album`
2. 仓库页面点 **Add file → Upload files**，把 `index.html`、`cover.jpg`、`icons` 文件夹拖进去，点 Commit
3. **Settings → Pages**，Source 选 `Deploy from a branch`，分支选 `main` / `(root)`，保存
4. 一两分钟后网址生效：`https://你的用户名.github.io/album/`
5. 把 `index.html` 里的 `<meta property="og:image" content="cover.jpg">`
   改成 `https://你的用户名.github.io/album/cover.jpg`，再上传一次

以后改内容只要重新上传 `index.html`，网址不变。

## 写入 NFC
- 贴片：NTAG215 或 NTAG216
- App：NFC Tools → 写 → 添加记录 → URL → 填上面的网址 → 写入
- iPhone 和安卓各测一次，没问题再考虑锁定（锁定后不能改）

## 语言测试
- `…/album/#zh` 强制中文，`…/album/#en` 强制英文
- 手动切换过的语言会被记住
