# 传奇文字 LegendWord

单文件 HTML 文字传奇游戏：凡界（封顶 170）→ 雷劫飞升 → 仙界 → 破界门 → 大世界（11 个「XX域」，200~1000 级）+ 灵器 / 专属灵器系统。

- 在线：<https://fornow330.github.io/legendword/>
- 备用：<https://fornow.cc>
- 作者：fornow
- 许可：GPL-3.0（全文见 `fornow330.github.io/legendword/LICENSE`）

## 说明

本仓库（`fornow330/legendword`）只作为项目名与指引入口，不存放游戏代码。加载器与发布资源位于 `fornow330/fornow330.github.io` 仓库的 `legendword/` 目录——GitHub Pages 用户站点必须由名为 `fornow330.github.io` 的仓库托管，游戏以子目录形式挂在同一站点下。

## 加载方式

加载器按顺序取回加密资源，校验通过后写入页面；取源回退顺序为 jsDelivr → 社区镜像 → 同站相对路径，所有来源按提交号钉版，避免 CDN 缓存导致新旧资源错配。
