# Logi Options Plus Mini

[中文](README.md) | [English](README_EN.md)

**Logi Options+ mini** 提供了一种选择来自定义 Logi Options+，方便用户能够更好地控制其功能。

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://github.com/user-attachments/assets/b39ddb4c-1f27-4673-9221-09c5f9e28b3d">
  <source media="(prefers-color-scheme: light)" srcset="https://github.com/user-attachments/assets/69ab444b-b9c0-4ee0-a889-bc4861313608">
  <img alt="Logi Options+ mini" src="https://github.com/user-attachments/assets/69ab444b-b9c0-4ee0-a889-bc4861313608" width="600" > 
</picture>

<img width="600" alt="image" src="https://github.com/Qetesh/logi-options-plus-mini/assets/4559341/d4c503a9-51d8-4a18-af90-a3f3be508e8b">
<img width="600" alt="image" src="https://github.com/Qetesh/logi-options-plus-mini/assets/4559341/14a85961-b022-4fc9-99bf-6e30b071f54c">
<img width="600" alt="image" src="https://github.com/Qetesh/logi-options-plus-mini/assets/4559341/bf97e703-d5d5-43d6-9236-6e1d06b7c0c8">
<img width="600" alt="image" src="https://github.com/user-attachments/assets/3afb9d21-242e-436d-af78-9d386d83bac4">


## 项目简介

参考官方[Logitech Options 软件的批量安装和配置](https://prosupport.logi.com/hc/zh-cn/articles/6046882446359-Logitech-Options-软件的批量安装和配置)

项目通过官方安装包命令行选项定制化Logi Options+功能。
支持macOS原生应用、macOS Shell、Windows PowerShell。

## 特性

- 定制化Logi Options+功能
- 易于使用的交互设计
- 卸载升级时自动保留配置
- 可定制功能
  - analytics 用户分享应用程序使用情况和诊断数据
  - flow
  - sso 用户登录应用程序的功能
  - update 应用程序更新
  - dfu 设备固件更新
  - logivoice 罗技语音功能
  - aipromptbuilder  AI Prompt Builder 功能（仅限macOS）
  - smartactions
  - actions-ring
  - device-recommendation 设备推荐功能（仅限macOS）

## 使用方法

### 使用 macOS 原生应用

下载最新版本 [here](https://v.qetesh.cc/d/Public/Logi%20Options%2B%20mini.dmg)

[<img width="64" alt="logi option plus1" src="https://github.com/user-attachments/assets/2c57172a-b1e3-4bab-abb8-6c60425ca640" />](https://v.qetesh.cc/d/Public/Logi%20Options%2B%20mini.dmg)

🔔 由于没有使用开发者证书签署应用，macOS可能会显示安全警告，需前往系统设置 → 隐私与安全 → 已阻止“Logi Options+mini”以保护Mac。然后点击“仍要打开”以运行该应用程序。

![WX20250305-181838@2x](https://github.com/user-attachments/assets/ca75fad3-b1e6-4b51-ba2c-f4b8e5770fb7)

### 使用 macOS Shell

1. 克隆此项目到本地

   ```bash
   git clone https://github.com/tjsky/logi-options-plus-mini.git
   cd logi-options-plus-mini
   ```
2. 运行Shell脚本（需要 `sudo`权限卸载旧版本）

  ```bash
  chmod u+x logi-options-plus-mini.command
  ./logi-options-plus-mini.command

  ##############################################################
  2024年12月15日 星期日 23时32分33秒 +08 | Starting install of Logi Options+
  ##############################################################

  Please select the features you want to keep:
  1. analytics:             Shows or hides choice for users to opt in to share app usage and diagnostics data.
  2. flow:                  Shows or hides the Flow feature. Default value is Yes
  3. sso:                   Shows or hides ability for users to sign into the app.
  4. update:                Enables or disables app updates.
  5. dfu:                   Enables or disables device firmware updates.
  6. backlight:             Enables or disables keyboard backlight on the supported keyboards.
  7. logivoice:             Enables or disables LogiVoice feature.
  8. aipromptbuilder:       Enables or disables AI Prompt Builder feature.
  9. device-recommendation: Enables or disables device recommendation feature.
  10. smartactions:         Enables or disables Smart Actions feature.
  11. actions-ring:         Enables or disables Actions Ring feature.
  12. all
  Press enter for none

  Enter your choices(e.g. 2 6, default is none): 
  ```
  
### 使用 Windows Shell

1. 克隆此项目到本地

   ```bash
   git clone https://github.com/tjsky/logi-options-plus-mini.git
   cd logi-options-plus-mini
   ```

2. 双击bat脚本 `Run_Install.bat`即可，(脚本会赋予临时的 ExecutionPolicy 权限)

  ```powershell
##############################################################
01/09/2026 10:48:24 | 开始安装 Logi Options+
##############################################################

01/09/2026 10:48:24 | 检测到您位于中国地区，使用 CN 下载源
01/09/2026 10:48:24 | 正在下载安装包: https://download.logitech.com.cn/web/ftp/pub/techsupport/optionsplus/logioptionsplus_installer.exe
01/09/2026 10:49:05 | 下载成功。

请选择你想保留/开启的功能：
0.  quiet:               静默安装（无人值守安装）
1.  analytics:           允许收集个人使用数据和诊断信息
2.  flow:                Flow 跨屏功能 (默认为 Yes)
3.  sso:                 启用 罗技账户 登录模块
4.  update:              启用 Logi Options+ 自动更新
5.  dfu:                 启用 设备固件 自动更新
6.  backlight:           启用 键盘背光 支持
7.  logivoice:           启用 罗技语音功能（LogiVoice）
8.  aipromptbuilder:     启用 AI 功能
9.  device-recommendation: 启用 新产品推荐（新产品广告）
10. smartactions:        启用 Smart Actions (按键宏)
11. actions-ring:        启用 Actions Ring（快捷启动）
12. all (全部开启)
直接按回车键，则执行最小化精简安装，不开启任何额外功能

如需自定义请输入选项 (例如 '0 2 6 10', 默认为 最小化精简安装): 0 5 6 10

  ```

脚本将会自动下载官方安装包，并进行精简安装。

## 系统要求

- macOS
- Windows
- 网络连接以下载官方安装包

## FAQ

- 部分Mac无法使用官方方式卸载，需使用第三方工具卸载后重新运行。已测试使用 `Pearcleaner`卸载后可正常运行安装

## 致谢 / 说明
- 本项目基于 [Qetesh](https://github.com/Qetesh) 的 [logi-options-plus-mini](https://github.com/Qetesh/logi-options-plus-mini) 修改开发。 感谢原作者的开源贡献。
- 分叉信息：由 [tjsky](https://github.com/tjsky) 分叉并修改：
 1. 添加windows系统下bat一键运行。
 2. 自动判断用户区域切换语言。
 3. 我没有mac打包环境，所以提供 macOS 原生应用为原作者的版本。

### Contributors
<a href="https://github.com/tjsky/logi-options-plus-mini/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=tjsky/logi-options-plus-mini" />
</a>


## 贡献

欢迎提交问题和请求。您可以通过以下方式贡献代码：

1. Fork 此仓库
2. 创建您的分支 (`git checkout -b feature/AmazingFeature`)
3. 提交您的更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 打开一个Pull Request


## 许可证

此项目使用 [Apache 许可证](LICENSE)。
