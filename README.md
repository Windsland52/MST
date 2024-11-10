<!-- markdownlint-disable MD033 MD041 -->

<p align="center">
  <img alt="LOGO" src="https://raw.githubusercontent.com/Windsland52/MST/refs/heads/dev/assets/resource/base/image/Logo/logo.jpg" width="256" height="256" />
</p>

<div align="center">

# MST

<!-- prettier-ignore-start -->
<!-- markdownlint-disable-next-line MD036 -->
_✨ 基于MaaFramework的灵魂潮汐(SoulTide)日常脚本 ✨_
<!-- prettier-ignore-end -->

</div>

<p align="center">
  <img alt="license" src="https://img.shields.io/github/license/Windsland52/MST">
  <img alt="platform" src="https://img.shields.io/badge/platform-Windows%20%7C%20Linux%20%7C%20macOS%20%7C%20Android-blueviolet">
  <img alt="commit" src="https://img.shields.io/github/commit-activity/m/Windsland52/MST?color=%23ff69b4">
  <img alt="stars" src="https://img.shields.io/github/stars/Windsland52/MST?style=social">
</p>

## 简介

基于全新架构的 灵魂潮汐 小助手。图像技术 + 模拟控制，解放双手！
由 [MaaFramework](https://github.com/MaaXYZ/MaaFramework) 强力驱动！

## 功能一览

- [x] 启动游戏
- [x] 每日签到
- [x] 领取邮件
- [x] 商店补给
- [x] 教会补给
- [x] 家园
  - [x] 炼金炉
  - [x] 种菜收菜
  - [x] 事务派遣
  - [x] 拜访好友（后续再写无好友版）
  - [x] 捕鱼（钓鱼后面再说）
- [ ] 战斗
  - [ ] 金币本扫荡
  - [ ] 主线
  - [ ] 异象(上榜)
- [ ] 巡查
- [x] 公会
- [ ] 相伴
  - [ ] 摸头
  - [ ] 送礼
- [ ] 每日抽卡
- [x] 任务/通行证
- [ ] 挖矿
- [x] 关闭游戏

## 使用说明

**[最新版下载地址](https://github.com/Windsland52/MST/releases/latest)**

### Windows

- 对于绝大部分用户，请下载 `MST-win-x86_64-vXXX.zip`
- 若确定自己的电脑是 arm 架构，请下载 `MST-win-aarch64-vXXX.zip`

> 请注意！Windows 的电脑几乎全都是 x86_64 的，可能占 99.999%，除非你非常确定自己是 arm，否则别下这个！

- 解压后运行 `MFAWPF.exe`（图形化界面）或 `MaaPiCli.exe`（命令行）即可

### macOS

- 若使用 Intel 处理器，请下载 `MST-macos-x86_64-vXXX.zip`
- 若使用 M1, M2 等 arm 处理器，请下载 `MST-macos-aarch64-vXXX.zip`
- 使用方式：

  ```bash
  chmod a+x MaaPiCli
  ./MaaPiCli
  ```

### Linux

~~用 Linux 的大佬应该不需要我教~~

## 其他说明

- 模拟器分辨率请选择 `1280*720`

- 提示“应用程序错误”，一般是缺少运行库，请安装一下 [vc_redist](https://aka.ms/vs/17/release/vc_redist.x64.exe)
- 添加 `-d` 参数可跳过交互直接运行任务，如 `./MaaPiCli.exe -d`
- 2.0 版本已支持 mumu 后台保活，会在 run task 时获取 mumu 最前台的 tab，并始终使用这个 tab（即使之后被切到后台了）
- 反馈问题请附上日志文件 `debug/maa.log` 以及问题界面的截图，谢谢！

## How to build

**如果你要编译源码才看这节，否则直接 [下载](https://github.com/Windsland52/MST/releases) 即可**

0. 完整克隆本项目及子项目

    ```bash
    git clone --recursive https://github.com/Windsland52/MST.git
    ```

1. 下载 `MaaFramework` 的 [Release 包](https://github.com/MaaXYZ/MaaFramework/releases)，解压到 `deps` 文件夹中
2. 安装

    ```python
    python ./install.py
    ```

生成的二进制及相关资源文件在 `install` 目录下

## 开发相关

- [MaaFW 开发思路](https://github.com/MaaXYZ/MaaFramework/blob/main/docs/zh_cn/1.1-%E5%BF%AB%E9%80%9F%E5%BC%80%E5%A7%8B.md#%E5%BC%80%E5%8F%91%E6%80%9D%E8%B7%AF)  
  MST 目前使用其中第一种方式（纯 Pipeline 低代码），后续可能会迁移到第二种方式（Pipeline + 自定义任务）
- [Pipeline 流水线协议](https://github.com/MaaXYZ/MaaFramework/blob/main/docs/zh_cn/3.1-%E4%BB%BB%E5%8A%A1%E6%B5%81%E6%B0%B4%E7%BA%BF%E5%8D%8F%E8%AE%AE.md)
- [开发日志](https://windsland52.github.io/)，可参考。

## 鸣谢

本项目由 **[MaaFramework](https://github.com/MaaXYZ/MaaFramework)** 强力驱动！

特别感谢 **[MFAWPF](https://github.com/SweetSmellFox/MFAWPF)** 提供的 GUI。

感谢以下开发者对本项目作出的贡献:

<a href="https://github.com/Windsland52/MST/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=Windsland52/MST&max=1000" />
</a>

## Join us

- MST开发/用户交流群 QQ 群：[212220209](http://qm.qq.com/cgi-bin/qm/qr?_wv=1027&k=zybZ5ST3IHx8_l8pajwFd9OxpNQzXjdy&authKey=C5qMnDOvB4mVKNNC%2By45eKc%2BLnETkm4XFQmmdrmWzu9qemKW4lurHbf4h4h8%2F0bA&noverify=0&group_code=212220209)