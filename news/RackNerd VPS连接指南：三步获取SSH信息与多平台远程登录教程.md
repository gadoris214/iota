# RackNerd VPS连接指南：三步获取SSH信息与多平台远程登录教程

成功部署RackNerd云主机后，获取正确的SSH连接信息是实现远程管理的关键步骤。本教程将详细介绍如何通过三种途径获取IP地址、SSH端口及root密码，并演示主流操作系统的连接方案。

## ▍SSH连接信息获取全流程

### 步骤1：查收系统邮件
完成VPS购买后，注册邮箱将收到标题为**"KVM VPS Login Information"**的系统邮件，其中包含：
- 服务器IP地址（IPv4 Address）
- SSH端口号（默认22）
- root账户初始密码

### 步骤2：后台信息验证
若未收到邮件，可通过RackNerd客户端的【View Email Log】功能追溯：
1. 登录控制面板
2. 在邮件日志中定位**VPS登录信息邮件**
3. 点击【View Message】查看完整连接参数

👉 [【建议收藏】2025年Racknerd最新优惠套餐整理汇总 - 每日更新可用活动优惠](https://bit.ly/Rack_Nerd)

### 步骤3：关键信息确认
建议首次登录后立即执行：
1. 通过`ping`命令验证IP连通性
2. 使用`ssh -p 端口号 root@IP地址`测试SSH连接
3. 执行`passwd`命令修改初始密码

## ▍多平台SSH连接方案

### Windows系统推荐
- **Xshell**：支持多会话管理/文件传输
- **PuTTY**：轻量级命令行工具

### macOS系统方案
- 终端直接执行：`ssh -p 端口号 root@服务器IP`
- 高级用户推荐安装Homebrew扩展工具包

### 移动端解决方案
- iOS：Termius（App Store评分4.8+）
- Android：JuiceSSH（Google Play超500万下载）

## ▍连接异常排查清单
当出现连接故障时，建议按顺序检查：
1. 防火墙是否开放指定SSH端口
2. 密码输入是否启用数字小键盘
3. VPS运行状态（通过控制面板确认）
4. 本地网络是否限制SSH协议

掌握这些核心技巧后，您已具备通过SSH协议管理RackNerd云服务的基础能力。建议定期更新系统组件（`yum update`/`apt update`）并配置SSH密钥认证以提升安全性。