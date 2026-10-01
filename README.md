# 尉迟公主 · 于阗（安卓壳）

这是一个最小的 WebView 壳工程：网页放在 `app/src/main/assets/www/index.html`，
云端构建由 `.github/workflows/build-apk.yml` 完成。

## 怎么出 APK（不用装 Android Studio）
1. 注册 GitHub 账号，新建一个仓库（Public 或 Private 都行）。
2. 把本文件夹里的**所有文件**上传上去（网页版 GitHub：Add file → Upload files，
   直接把文件夹拖进去即可，注意保持目录结构，尤其是 `.github` 文件夹）。
3. 打开仓库的 **Actions** 标签页，等 1–3 分钟，看到绿色的勾。
4. 点进那次构建 → 页面底部 **Artifacts** → 下载 `yutian-apk` → 解压得到 `app-debug.apk`。
5. 把这个 APK 发到手机上安装（允许“未知来源”即可）。

## 想改游戏内容
只改 `app/src/main/assets/www/index.html` 就行，改完提交，Actions 会自动重新构建。

## 说明
- 不需要任何权限，不联网也能玩。
- 用的是 debug 签名，自己装着玩没问题；要在商店上架需要换成正式签名。
