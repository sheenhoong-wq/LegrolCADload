# LegrolCADload

LegrolCAD 安卓版的发布仓库，只存 APK，不含源码。

- 每个 Release 的 tag 形如 `v0.6.0-b12`：`0.6.0` 是版本号，`b12` 是打包时的 Actions run 编号（也是 APK 的 versionCode）。
- app 内「检查更新」查的就是这里的 `releases/latest`，有新 build 会提示下载安装。
- 由源码仓库 LegrolCAD 的 Actions（Build APK，勾 release）自动发布，不要手动改这里。

## 法律文本（GitHub Pages）

`docs/` 同时是 GitHub Pages 的站点根，挂着 app 里链接的两份文本：

- 服务条款 https://sheenhoong-wq.github.io/LegrolCADload/terms
- 隐私政策 https://sheenhoong-wq.github.io/LegrolCADload/privacy

这两个 HTML 是**生成物**，源文件在源码仓库 LegrolCAD 的 `docs/legal/*.md`。
要改内容就改那边，跑 `python3 docs/legal/build_site.py` 重新生成，再把
`docs/legal/site/` 里的内容覆盖到这里的 `docs/`。别直接改这里的 HTML。

Pages 设置：Settings → Pages → Deploy from a branch → `main` / `/docs`。
