# 传奇文字 LegendWord

单文件 HTML 文字传奇游戏：凡界（封顶 170）→ 雷劫飞升 → 仙界 → 破界门 → 大世界（11 个「XX域」，200~1000 级）+ 灵器 / 专属灵器系统。

## 在线玩

- 游戏入口：https://fornow330.github.io/legendword/
- 云端备用：https://vcn2hg0t34as.doubao.link/app/app_17j122qqdfb

## 说明

本仓库（`fornow330/legendword`）只作为项目名与指引入口，**不存放游戏代码**。

游戏源码、加载器与全部压缩分片位于：

- 仓库：https://github.com/fornow330/fornow330.github.io
- 目录：`legendword/index.html`（加载器）+ `legendword/c00 ~ c11`（游戏本体，gzip + base64 分片）

之所以放在 `.github.io` 仓库：GitHub Pages 用户站点必须由名为 `fornow330.github.io` 的仓库托管，游戏以子目录形式挂在同一站点下，访问路径即项目名。

## 加载方式

加载器依次取回 c00 → c11 分片，拼接后 gzip 解压，再写入页面；取片按四级回退：

1. `fastly.jsdelivr.net/gh/fornow330/fornow330.github.io@<提交号>`
2. `ghproxy.net` 镜像
3. `gh-proxy.com` 镜像
4. 同目录相对路径（GitHub Pages 原生）

以上来源均按提交号钉版，避免 CDN 缓存与新旧分片错配。
