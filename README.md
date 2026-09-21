# LegrolCADload

LegrolCAD 安卓版的发布仓库，只存 APK，不含源码。

- 每个 Release 的 tag 形如 `v0.6.0-b12`：`0.6.0` 是版本号，`b12` 是打包时的 Actions run 编号（也是 APK 的 versionCode）。
- app 内「检查更新」查的就是这里的 `releases/latest`，有新 build 会提示下载安装。
- 由源码仓库 LegrolCAD 的 Actions（Build APK，勾 release）自动发布，不要手动改这里。
