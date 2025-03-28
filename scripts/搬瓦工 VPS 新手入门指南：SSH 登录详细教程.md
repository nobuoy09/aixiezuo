# 搬瓦工 VPS 新手入门指南：SSH 登录详细教程

对于刚接触 VPS 的新手来说，SSH 登录可能是第一个需要掌握的技能。本文将详细介绍如何使用 SSH 连接到搬瓦工 VPS，涵盖 Windows、Linux、macOS 和移动设备等多种平台的操作方法。

## 一、获取 SSH 登录所需信息

登录 VPS 需要以下关键信息：

1. **IP 地址**：VPS 的公网 IP
2. **SSH 端口**：默认是 22，但搬瓦工通常会随机生成
3. **用户名和密码**：通常是 root 账户和密码

### 如何获取这些信息？

1. 登录 KiwiVM 控制面板
2. 查看"Public IP address"和"SSH Port"字段
3. 如果没有收到密码邮件，可以在控制面板中重置密码：
   - 选择"Root password modification"
   - 点击"Generate and set new root password"

> 注意：重置密码时需要保持 VPS 处于开机状态

👉 [【点击查看】2025年最新 BandwagonHost 搬瓦工优惠码及特价云服务器方案汇总](https://bit.ly/banwagon)

## 二、各平台 SSH 登录方法

### Windows 用户

推荐使用以下 SSH 客户端：
- FinalShell（功能全面，推荐首选）
- 宝塔远程工具（简单易用）

两款软件都有免费版本，基本功能完全够用。

### Linux/macOS 用户

1. 打开终端
2. 输入命令：
   bash
   ssh -p 端口号 root@IP地址
   
3. 输入密码即可连接

也可以使用跨平台的 Termius 客户端。

### 移动设备用户

推荐使用 Termius 应用：
1. 在应用商店下载 Termius
2. 添加新的 SSH 连接
3. 输入 IP、端口、用户名和密码
4. 保存并连接

## 三、套餐选择建议

根据需求选择合适的搬瓦工套餐：
- **入门级**：洛杉矶 CN2 GT 套餐，价格实惠
- **推荐款**：洛杉矶 CN2 GIA-E 套餐，性能优异，性价比高
- **高端选择**：香港 CN2 GIA 套餐，网络质量最佳

掌握 SSH 登录是使用 VPS 的第一步，希望本教程能帮助新手顺利开始 VPS 之旅。