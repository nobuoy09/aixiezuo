# AdsPower 本地API与无头浏览器模式详解

本文将详细介绍如何通过API密钥和"headless"参数在AdsPower中实现无头浏览器模式运行，并充分利用本地API功能。

## 无头模式与API密钥解析

- **无头模式(headless)**：通过特殊参数实现浏览器后台运行的技术
- **API密钥**：用于本地API身份验证的唯一标识符，支持多设备同时使用

> 注意：此功能仅对拥有本地API访问权限的用户开放。如需开通请联系客服。

## 无头模式操作指南

### 第一步：获取API密钥

1. 打开AdsPower客户端
2. 进入"账户管理 → 设置"
3. 在"本地API"区域点击"生成api-key"
4. 复制生成的API密钥

### 第二步：通过命令行启动无头模式

1. 在AdsPower安装目录打开CMD/Terminal
   - Windows默认路径：`C:\Program Files (x86)\AdsPower`
   - Mac默认路径：`/Applications/adsPower.app/Contents/MacOS/`

2. 执行相应命令：
   - **Windows**：
     bash
     AdsPower.exe --headless=true --api-key=XXXX --api-port=50325
     
   - **MacOS**：
     bash
     /Applications/adsPower.app/Contents/MacOS/Adspower --args --headless=true --api-key=XXXX --api-port=50325
     

执行成功后，系统将返回本地API的访问地址。

👉 [【点击查看】2025年最新 AdsPower优惠码及特价活动方案汇总](https://bit.ly/adspower_free)

## 模式对比：有头 vs 无头

| 特性 | 有头模式 | 无头模式 |
|------|---------|---------|
| 设备限制 | 单设备登录 | 多设备同时登录 |
| 自动化支持 | 有限 | 完整API支持 |
| 资源占用 | 较高 | 较低 |

无头模式特别适合需要：
- 多设备自动化操作
- 后台静默运行
- 大规模账号管理

## 常见问题解答

**Q：能否同时运行有头和无头模式？**
A：不支持同时运行两种模式。

**Q：API密钥变更后，旧密钥是否仍有效？**
A：无效。系统会提示密钥错误，每个账户同一时间只能有一个有效API密钥。

**Q：如何重置API密钥？**
A：进入"账户管理→设置"，点击"生成api-key"获取新密钥。

**Q：无头模式下能否直接更新API密钥？**
A：不可以。需要先退出无头模式，使用新密钥重新启动。

如需了解更多高级功能或获取技术支持，请访问[AdsPower官方网站](https://bit.ly/adspower_free)。