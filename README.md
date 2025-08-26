<!-- markdownlint-configure-file {
  "MD013": { "code_blocks": false, "tables": false, "line_length":200 },
  "MD033": false,
  "MD041": false
} -->

[license]: /LICENSE
[license-badge]: https://img.shields.io/github/license/zhiern/luci-theme-argon?style=flat-square&a=1
[prs]: https://github.com/zhiern/luci-theme-argon/pulls
[prs-badge]: https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square
[issues]: https://github.com/zhiern/luci-theme-argon/issues/new
[issues-badge]: https://img.shields.io/badge/Issues-welcome-brightgreen.svg?style=flat-square
[release]: https://github.com/zhiern/luci-theme-argon/releases
[release-badge]: https://img.shields.io/github/v/release/zhiern/luci-theme-argon?style=flat-square
[download]: https://github.com/zhiern/luci-theme-argon/releases
[download-badge]: https://img.shields.io/github/downloads/zhiern/luci-theme-argon/total?style=flat-square

<div align="center">
<img src="https://raw.githubusercontent.com/jerrykuku/staff/master/argon_title4.svg">

# 一个简洁优雅的 OpenWrt 主题

Argon 是**一款基于 LuCI 的 OpenWrt 主题**，  
支持深色/浅色模式切换，自定义登录背景（图片或视频），  
并配合 [luci-app-argon-config](https://github.com/zhiern/luci-theme-argon) 插件提供更多个性化设置。

[![license][license-badge]][license]
[![prs][prs-badge]][prs]
[![issues][issues-badge]][issues]
[![release][release-badge]][release]
[![download][download-badge]][download]

**简体中文**

[特色](#特色) •
[分支介绍](#分支介绍) •
[快速开始](#快速开始) •
[注意](#注意) •
[屏幕截图](#屏幕截图) •
[贡献者](#贡献者) •
[鸣谢](#鸣谢)

</div>

---

## 特色

- 简洁现代的 UI 设计，优化桌面端与移动端体验。
- 自动/手动切换浅色与深色模式。
- 自定义主题颜色。
- 支持设置 Bing 每日壁纸为登录背景。
- 支持上传图片或视频作为登录背景。
- 配套设置插件 [luci-app-argon-config](https://github.com/zhiern/luci-theme-argon)。

## 分支介绍

| 分支          | 版本   | 说明                        | 适配源码                  |
| ------------- | ------ | --------------------------- | ------------------------- |
| `openwrt-24.10` | v2.x.x | 支持 OpenWrt 官方 24.10+    | [OpenWrt 官方](https://github.com/openwrt/openwrt) |

## 快速开始

### 源码构建

在 **OpenWrt / ImmortalWrt** 源码环境中：

```bash
cd openwrt/package
git clone -b openwrt-24.10 https://github.com/zhiern/luci-theme-argon.git
make menuconfig # LUCI -> Themes -> luci-theme-argon
make -j$(nproc)
```

### 手动安装 ipk

从 [Releases](https://github.com/zhiern/luci-theme-argon/releases) 下载对应版本的 ipk：

```bash
opkg install luci-theme-argon*.ipk
opkg install luci-app-argon-config*.ipk
```

### 在官方和 ImmortalWrt 上安装

```bash
opkg install luci-compat
opkg install luci-lib-ipkg
wget --no-check-certificate https://github.com/zhiern/luci-theme-argon/releases/download/v2.4.2/luci-theme-argon_2.4.2-r20250207_all.ipk
opkg install luci-theme-argon*.ipk
```

### 安装 luci-app-argon-config

```bash
wget --no-check-certificate https://github.com/zhiern/luci-theme-argon/releases/download/v2.4.2/luci-app-argon-config_1.0-r20230608_all.ipk
opkg install luci-app-argon-config*.ipk
```

## 注意

- 强烈建议使用 Chrome 浏览器。这个主题中使用了一些新的 css3 功能，目前只有 Chrome 浏览器有最好的兼容性。
- 微软已正式退役 Internet Explorer，安息吧 IE🙏<del>目前，IE 系列的主线版本有需要解决的错误。</del>
- FireFox 默认不启用 backdrop-filter，[见这里](https://developer.mozilla.org/zh-CN/docs/Web/CSS/backdrop-filter)的打开方法。

## 屏幕截图

![desktop](https://git.kejizero.online/zhao/image/raw/branch/main/10.png)
![mobile](https://git.kejizero.online/zhao/image/raw/branch/main/11.png)

## 贡献者

<a href="https://github.com/zhiern/luci-theme-argon/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=zhiern/luci-theme-argon" />
</a>

Made with [contrib.rocks](https://contrib.rocks).

## 鸣谢

[luci-theme-material](https://github.com/LuttyYang/luci-theme-material/)
