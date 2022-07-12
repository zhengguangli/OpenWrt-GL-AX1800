# GL-AX1800 & GL-AXT1800 固件

[![](https://img.shields.io/github/release-date/Draco-china/Draco-OpenWrt-GL-AX1800?label=固件更新&style=flat-square)](https://github.com/Draco-china/Draco-OpenWrt-GL-AX1800/actions)
[![](https://img.shields.io/badge/仓库地址-点我-brightgreen?style=flat-square)](https://github.com/draco-china/Draco-OpenWrt-GL-AX1800)
[![](https://img.shields.io/badge/固件下载-点我-brightgreen?style=flat-square)](https://github.com/draco-china/Draco-OpenWrt-GL-AX1800/releases)
[![](https://img.shields.io/badge/QQ群-303121713-brightgreen?style=flat-square)](https://jq.qq.com/?_wv=1027&k=JVYytZpL)

![](https://img.shields.io/badge/主要功能:-blueviolet.svg?style=flat-square) ![](https://img.shields.io/badge/-OpenClash-blue.svg?style=flat-square) ![](https://img.shields.io/badge/-AdGuard_Home-blue.svg?style=flat-square) ![](https://img.shields.io/badge/-Samba-blue.svg?style=flat-square) ![](https://img.shields.io/badge/-CIFSD-blue.svg?style=flat-square) ![](https://img.shields.io/badge/-FTP-blue.svg?style=flat-square) ![](https://img.shields.io/badge/-SFTP-blue.svg?style=flat-square) ![](https://img.shields.io/badge/-DLNA-blue.svg?style=flat-square) ![](https://img.shields.io/badge/-Aria2-blue.svg?style=flat-square) ![](https://img.shields.io/badge/-Transmission-blue.svg?style=flat-square) ![](https://img.shields.io/badge/-解锁网易云灰色歌曲-blue.svg?style=flat-square) ![](https://img.shields.io/badge/-UPnP-blue.svg?style=flat-square) ![](https://img.shields.io/badge/-京东签到服务-blue.svg?style=flat-square) ![](https://img.shields.io/badge/-IPv6_加速-blue.svg?style=flat-square) ![](https://img.shields.io/badge/-BBR_加速-blue.svg?style=flat-square) ![](https://img.shields.io/badge/-FullCone_NAT_加速-blue.svg?style=flat-square) ![](https://img.shields.io/badge/-SFE_加速-blue.svg?style=flat-square) ![](https://img.shields.io/badge/-HWNAT_加速-blue.svg?style=flat-square) ![](https://img.shields.io/badge/-桥接加速-blue.svg?style=flat-square) ![](https://img.shields.io/badge/-DDNS-blue.svg?style=flat-square) ![](https://img.shields.io/badge/-Docker_容器-blue.svg?style=flat-square) ![](https://img.shields.io/badge/-Frpc_NPS_内网穿透-blue.svg?style=flat-square) ![](https://img.shields.io/badge/-多线多拨-blue.svg?style=flat-square) ![](https://img.shields.io/badge/-负载均衡-blue.svg?style=flat-square) ![](https://img.shields.io/badge/-SQM_Qos-blue.svg?style=flat-square) ![](https://img.shields.io/badge/-文件助手-blue.svg?style=flat-square) ![](https://img.shields.io/badge/-文件浏览器-blue.svg?style=flat-square) ![](https://img.shields.io/badge/-可道云-blue.svg?style=flat-square) ![](https://img.shields.io/badge/-Rclone-blue.svg?style=flat-square) ![](https://img.shields.io/badge/-SmartDNS-blue.svg?style=flat-square) ![](https://img.shields.io/badge/-网络唤醒-blue.svg?style=flat-square) ![](https://img.shields.io/badge/-TTYD_终端-blue.svg?style=flat-square) ![](https://img.shields.io/badge/-迅雷快鸟-blue.svg?style=flat-square) ![](https://img.shields.io/badge/-USB_打印服务器-blue.svg?style=flat-square) ![](https://img.shields.io/badge/-KMS_服务器-blue.svg?style=flat-square) ![](https://img.shields.io/badge/-微信推送-blue.svg?style=flat-square) ![](https://img.shields.io/badge/-上网时间控制-blue.svg?style=flat-square) ![](https://img.shields.io/badge/-WatchCat-blue.svg?style=flat-square) ![](https://img.shields.io/badge/-各种驱动-blue.svg?style=flat-square) ![](https://img.shields.io/badge/-DNS_Filter-blue.svg?style=flat-square) ![](https://img.shields.io/badge/-持续更新中……-blue.svg?style=flat-square)

## 目录介绍

```tree
Draco-OpenWrt-GL-AX1800
├── .github/workflows
│   ├── build-glnet-ax1800.yml    云编译 AX1800
│   ├── build-glnet-axt1800.yml   云编译 AXT1800
│   ├── generate-glinet.yml       云生成 `glinet-ax1800.yml` & `glinet-ax1800.yml`
├── scripts
│   ├── build.sh                  本地编译脚本，必须在项目根目录下执行 `./scripts/build.sh`
│   ├── feeds.js                  feeds 第三方仓库地址配置
│   ├── generate.js               云生成 `glinet-ax1800.yml` & `glinet-ax1800.yml` 脚本
│   └── packages.js               packages 第三方软件包配置
├── glinet-ax1800.yml             AX1800 编译描述文件
├── glinet-axt1800.yml            AXT1800 编译描述文件
└── README.md
```

## 其他说明

- *基于官方编译器 <https://github.com/gl-inet/gl-infra-builder> 构建, 支持官方界面*
- *通过  openwrt-ipq807x-glinet_ax1800-squashfs-sysupgrade.tar 升级*
- *进入uboot，选择openwrt-ipq807x-glinet_ax1800-squashfs-nand-factory.img 文件升级*
- 部分 `feeds` & `packages` 已经注释移除，可自行 `fork` 编译定制
- 北京时间每天 `23:00` 定时更新 `glinet-ax1800.yml` & `glinet-axt1800.yml`
- 北京时间每天 `0:00` 定时编译，`Release` 中只保留最新版本
- 历史版本在 `Actions` 中选择一个已经运行完成且成功的 `workflow` 在页面底部可以看到 `Annotations` 和 `Artifacts`
- `Annotations` 中的网盘失效时间一般是 1-3 天, `Artifacts` 需要登录 Github 才能下载
- `Actions` 运行需要设置 `Actions Secrets`, 查看[配置令牌](#配置令牌)

## 配置令牌

- 创建 [Personal access token(PAT)](https://github.com/settings/tokens/new) ，勾选repo权限，这将用于自动触发编译工作流程。
- ![](./preview/WX20220711-202547%402x.png)
- 然后点击自己仓库的Settings选项卡，再点击Secrets。添加名为ACTIONS_TRIGGER_PAT的加密环境变量，保存刚刚创建的 PAT 。
- ![](./preview/WX20220711-202739%402x.png)
- 在 Actions 页面选择Update Checker，点击Run workflow手动进行一次测试运行。如果没有报错且 OpenWrt 编译工作流程被触发，则代表测试通过。
- 最后编辑Update Checker的 workflow 文件（.github/workflows/update-checker.yml），取消注释（删除#）定时触发相关的部分。这里可以根据 cron 格式来设定检测的时间，时区为 UTC 。

## 界面一览

![](./preview/WX20220709-153420@2x.png)
![](./preview/WX20220709-151127%402x.png)

## Credits

- [Microsoft Azure](https://azure.microsoft.com)
- [GitHub Actions](https://github.com/features/actions)
- [OpenWrt](https://github.com/openwrt/openwrt)
- [Lean's OpenWrt](https://github.com/coolsnowwolf/lede)
- [tmate](https://github.com/tmate-io/tmate)
- [mxschmitt/action-tmate](https://github.com/mxschmitt/action-tmate)
- [csexton/debugger-action](https://github.com/csexton/debugger-action)
- [Cowtransfer](https://cowtransfer.com)
- [WeTransfer](https://wetransfer.com/)
- [Mikubill/transfer](https://github.com/Mikubill/transfer)
- [softprops/action-gh-release](https://github.com/softprops/action-gh-release)
- [ActionsRML/delete-workflow-runs](https://github.com/ActionsRML/delete-workflow-runs)
- [dev-drprasad/delete-older-releases](https://github.com/dev-drprasad/delete-older-releases)
- [peter-evans/repository-dispatch](https://github.com/peter-evans/repository-dispatch)
- [P3TERX/Actions-OpenWrt](https://github.com/P3TERX/Actions-OpenWrt)
- [gl-inet/gl-infra-builder](https://github.com/gl-inet/gl-infra-builder)
- [JiaY-shi/build-gl](https://github.com/JiaY-shi/build-gl.inet)

## License

[MIT](https://github.com/P3TERX/Actions-OpenWrt/blob/main/LICENSE) © [**P3TERX**](https://p3terx.com)
