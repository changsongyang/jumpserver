<div align="center">
  <a name="readme-top"></a>
  <a href="https://jumpserver.com" target="_blank"><img src="https://download.jumpserver.org/images/jumpserver-logo.svg" alt="JumpServer" width="300" /></a>
  
## 一個開源的 PAM 工具 (堡壘主機)

</div>
<br/>

## 什麼是 JumpServer？

JumpServer 是一個開源的特權訪問管理 (PAM) 工具，為 DevOps 和 IT 團隊通過網頁瀏覽器提供隨需而且安全的 SSH、RDP、Kubernetes、數據庫和 RemoteApp 終端的訪問。

![JumpServer 概覽](https://github.com/jumpserver/jumpserver/assets/32935519/35a371cb-8590-40ed-88ec-f351f8cf9045)

## 快速開始

準備一台乾淨的 Linux 伺服器 (64 位，>= 4c8g)

```sh
curl -sSL https://github.com/jumpserver/jumpserver/releases/latest/download/quick_start.sh | bash
```

在瀏覽器中訪問 JumpServer，網址為 `http://your-jumpserver-ip/`
- 使用者名稱：`admin`
- 密碼：`ChangeMe`

[![JumpServer 快速開始](https://github.com/user-attachments/assets/0f32f52b-9935-485e-8534-336c63389612)](https://www.youtube.com/watch?v=UlGYRbKrpgY "JumpServer 快速開始")

## 截圖

<table style="border-collapse: collapse; border: 1px solid black;">
  <tr>
    <td style="padding: 5px;background-color:#fff;"><img src= "https://github.com/jumpserver/jumpserver/assets/32935519/99fabe5b-0475-4a53-9116-4c370a1426c4" alt="JumpServer 控制台"   /></td>
    <td style="padding: 5px;background-color:#fff;"><img src= "https://github.com/jumpserver/jumpserver/assets/32935519/a424d731-1c70-4108-a7d8-5bbf387dda9a" alt="JumpServer 審計"   /></td>
  </tr>

  <tr>
    <td style="padding: 5px;background-color:#fff;"><img src= "https://github.com/jumpserver/jumpserver/assets/32935519/393d2c27-a2d0-4dea-882d-00ed509e00c9" alt="JumpServer 工作臺"   /></td>
    <td style="padding: 5px;background-color:#fff;"><img src= "https://github.com/jumpserver/jumpserver/assets/32935519/3a2611cd-8902-49b8-b82b-2a6dac851f3e" alt="JumpServer 設置"   /></td>
  </tr>

  <tr>
    <td style="padding: 5px;background-color:#fff;"><img src= "https://github.com/jumpserver/jumpserver/assets/32935519/1e236093-31f7-4563-8eb1-e36d865f1568" alt="JumpServer SSH"   /></td>
    <td style="padding: 5px;background-color:#fff;"><img src= "https://github.com/jumpserver/jumpserver/assets/32935519/69373a82-f7ab-41e8-b763-bbad2ba52167" alt="JumpServer RDP"   /></td>
  </tr>
  <tr>
    <td style="padding: 5px;background-color:#fff;"><img src= "https://github.com/jumpserver/jumpserver/assets/32935519/5bed98c6-cbe8-4073-9597-d53c69dc3957" alt="JumpServer K8s"   /></td>
    <td style="padding: 5px;background-color:#fff;"><img src= "https://github.com/jumpserver/jumpserver/assets/32935519/b80ad654-548f-42bc-ba3d-c1cfdf1b46d6" alt="JumpServer DB"   /></td>
  </tr>
</table>

## 組件

JumpServer 由多個關鍵組件組成，這些組件共同組成 JumpServer 的功能框架，為用戶提供綜合的運營管理和安全控制能力。

| 專案                                                | 狀態                                                                                                                                                                 | 描述                                                                                             |
|---------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|
| [Lina](https://github.com/jumpserver/lina)        | <a href="https://github.com/jumpserver/lina/releases"><img alt="Lina release" src="https://img.shields.io/github/release/jumpserver/lina.svg" /></a>                   | JumpServer 網頁 UI                                                                                 |
| [Luna](https://github.com/jumpserver/luna)        | <a href="https://github.com/jumpserver/luna/releases"><img alt="Luna release" src="https://img.shields.io/github/release/jumpserver/luna.svg" /></a>                   | JumpServer 網頁終端                                                                                 |
| [KoKo](https://github.com/jumpserver/koko)        | <a href="https://github.com/jumpserver/koko/releases"><img alt="Koko release" src="https://img.shields.io/github/release/jumpserver/koko.svg" /></a>                   | JumpServer 字符協議連接器                                                                           |
| [Lion](https://github.com/jumpserver/lion)        | <a href="https://github.com/jumpserver/lion/releases"><img alt="Lion release" src="https://img.shields.io/github/release/jumpserver/lion.svg" /></a>                   | JumpServer 圖形協議連接器                                                                           |
| [Chen](https://github.com/jumpserver/chen)        | <a href="https://github.com/jumpserver/chen/releases"><img alt="Chen release" src="https://img.shields.io/github/release/jumpserver/chen.svg" />                       | JumpServer 網頁數據庫                                                                                 |  
| [Tinker](https://github.com/jumpserver/tinker)    | <img alt="Tinker" src="https://img.shields.io/badge/release-private-red" />                                                                                            | JumpServer 遠程應用連接器 (Windows)                                                          |
| [Panda](https://github.com/jumpserver/Panda)      | <img alt="Panda" src="https://img.shields.io/badge/release-private-red" />                                                                                             | JumpServer EE 遠程應用連接器 (Linux)                                                             |
| [Razor](https://github.com/jumpserver/razor)      | <img alt="Chen" src="https://img.shields.io/badge/release-private-red" />                                                                                              | JumpServer EE RDP 代理連接器                                                                      |
| [Magnus](https://github.com/jumpserver/magnus)    | <img alt="Magnus" src="https://img.shields.io/badge/release-private-red" />                                                                                            | JumpServer EE 數據庫代理連接器                                                                    |
| [Nec](https://github.com/jumpserver/nec)          | <img alt="Nec" src="https://img.shields.io/badge/release-private-red" />                                                                                               | JumpServer EE VNC 代理連接器                                                                       |
| [Facelive](https://github.com/jumpserver/facelive)| <img alt="Facelive" src="https://img.shields.io/badge/release-private-red" />                                                                                          | JumpServer EE 面部識別                                                                            |


## 貢獻

歡迎提交 PR 來貢獻。請參考 [CONTRIBUTING.md][contributing-link] 獲取指導。

## 安全

JumpServer 是一個關鍵任務產品。請參考基本安全建議以進行安裝和部署。如果您遇到任何與安全相關的問題，請直接與我們聯繫：

- 電子郵件：support@fit2cloud.com

## License

Copyright (c) 2014-2025 FIT2CLOUD, All rights reserved.

Licensed under The GNU General Public License version 3 (GPLv3) (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at

https://www.gnu.org/licenses/gpl-3.0.html

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an " AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.

<!-- JumpServer official link -->
[docs-link]: https://jumpserver.com/docs
[discord-link]: https://discord.com/invite/W6vYXmAQG2
[contributing-link]: https://github.com/jumpserver/jumpserver/blob/dev/CONTRIBUTING.md

<!-- JumpServer Other link-->
[license-link]: https://www.gnu.org/licenses/gpl-3.0.html
[docker-link]: https://hub.docker.com/u/jumpserver
[github-release-link]: https://github.com/jumpserver/jumpserver/releases/latest
[github-stars-link]: https://github.com/jumpserver/jumpserver
[github-issues-link]: https://github.com/jumpserver/jumpserver/issues

<!-- Shield link-->
[github-release-shield]: https://img.shields.io/github/v/release/jumpserver/jumpserver
[github-stars-shield]: https://img.shields.io/github/stars/jumpserver/jumpserver?color=%231890FF&style=flat-square
[docker-shield]: https://img.shields.io/docker/pulls/jumpserver/jms_all.svg
[license-shield]: https://img.shields.io/github/license/jumpserver/jumpserver
[discord-shield]: https://img.shields.io/discord/1194233267294052363?style=flat&logo=discord&logoColor=%23f5f5f5&labelColor=%235462eb&color=%235462eb

<!-- Image link -->