# YTDLP Studio Runtime

本仓库公开发布 YTDLP Studio 的跨平台运行组件，不包含应用核心源码、用户数据、媒体文件或下载记录。

## 内容

每个 Release 由 GitHub Actions 在对应原生系统构建，按平台提供 FFmpeg、FFprobe、aria2c、yt-dlp。Windows 组件包同时包含已验证可加载的 libmpv 及其必需 DLL 依赖；组件用于应用的环境检测、自动修复和离线迁移。

## 覆盖平台

- Windows x64 / ARM64
- macOS Intel / Apple Silicon
- Linux x64 / ARM64

## 发布方式

在 **Actions → Build Runtime Components → Run workflow** 输入版本号即可发布组件归档。应用核心构建在私有的 `YTDLP-Studio-Core` 仓库完成；两者保持严格分离。

## 不包含的内容

- YTDLP Studio 应用源码或私有桌面安装包
- 用户 Cookie、账户信息、设置、预设与任务数据
- 已下载媒体、缓存、日志或转码临时文件
