<div align="center">

# 📊 SubsTracker

**订阅管理与提醒系统 - 轻量级订阅追踪工具**

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![GitHub Stars](https://img.shields.io/github/stars/Yeshenyue11/subscription-manager?style=social)](https://github.com/Yeshenyue11/subscription-manager/stargazers)
[![Deploy to Cloudflare](https://deploy.workers.cloudflare.com/button)](https://deploy.workers.cloudflare.com/?url=https://github.com/Yeshenyue11/subscription-manager)

[![Cloudflare Workers](https://img.shields.io/badge/Cloudflare-Workers-F38020?style=flat&logo=cloudflare&logoColor=white)](https://workers.cloudflare.com/)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)](https://www.javascript.com/)
[![Telegram](https://img.shields.io/badge/Telegram-2CA5E0?style=flat&logo=telegram&logoColor=white)](https://telegram.org/)

</div>

---

## 💡 简介

基于 **Cloudflare Workers** 的轻量级订阅管理系统，帮助您轻松跟踪各类订阅服务的到期时间，并通过 **Telegram、Webhook** 等多渠道发送及时提醒。

![SubsTracker Preview](https://github.com/user-attachments/assets/22ff1592-7836-4f73-aa13-24e9d43d7064)

---

## ✨ 功能特色

### 🎯 核心功能

| 功能 | 描述 |
|------|------|
| 📋 **订阅管理** | 添加、编辑、删除各类订阅服务 |
| ⏰ **智能提醒** | 自定义提前提醒天数，自动续订计算 |
| 🌙 **农历显示** | 支持农历日期显示，可控制开关 |
| 🔛 **状态管理** | 订阅启用/停用，过期状态自动识别 |
| 💰 **财务追踪** | 记录订阅费用，完整的支付历史和统计分析 |
| 📊 **仪表盘** | 可视化展示月度/年度支出，支出趋势和分类统计 |

### 📱 多渠道通知

- **Telegram** - Telegram Bot 通知
- **NotifyX** - 集成 NotifyX 推送服务
- **Webhook** - 自定义 Webhook 推送
- **企业微信** - 企业微信群机器人通知
- **邮件** - 基于 Resend 的专业邮件服务
- **Bark** - iOS Bark 推送

### 🎨 用户体验

- ✅ 响应式设计，完美适配桌面端和移动端
- ✅ 支持浅色/深色模式，跟随系统自动切换
- ✅ 实时预览，日期选择时显示农历
- ✅ 记住用户偏好设置

---

## 🚀 快速开始

### 一键部署

[![Deploy to Cloudflare Workers](https://deploy.workers.cloudflare.com/button)](https://deploy.workers.cloudflare.com/?url=https://github.com/Yeshenyue11/subscription-manager)

### 三步开始

#### 1️⃣ 部署
点击上方部署按钮，创建 KV 命名空间 `SUBSCRIPTIONS_KV`

#### 2️⃣ 登录
- 默认用户名：`admin`
- 默认密码：`password`

#### 3️⃣ 配置
1. 修改默认密码
2. 配置通知渠道
3. 添加订阅并设置提醒

---

## 📋 手动部署

### 1. 创建 Worker

在 Cloudflare 控制台创建 Worker，粘贴 `index.js` 代码

### 2. 创建 KV 命名空间

创建名为 `SUBSCRIPTIONS_KV` 的 KV 命名空间

### 3. 绑定配置

- 绑定 KV 命名空间到 Worker
- 设置 Cron 定时任务（推荐：`0 0 * * *` 每天 UTC 0:00）

### 4. 登录配置

访问部署域名，使用默认账号登录并配置通知

---

## 🔧 通知配置

### Telegram Bot

| 配置项 | 获取方式 |
|--------|----------|
| Bot Token | [@BotFather](https://t.me/BotFather) |
| Chat ID | [@userinfobot](https://t.me/userinfobot) |

### 其他渠道

详见系统内置配置说明

---

## 📊 功能截图

<details>
<summary>点击展开查看更多截图</summary>

### 仪表盘
![Dashboard](https://github.com/user-attachments/assets/f6db2089-28a1-439d-9de0-412ee4b2807f)

### 订阅列表
![Subscription List](https://github.com/user-attachments/assets/5dac1ce0-43a3-4642-925c-d9cf21076454)

### 支付历史
![Payment History](https://github.com/user-attachments/assets/af530379-332c-4482-9e6e-229a9e24775e)

</details>

---

## 🛠️ 技术栈

- **Cloudflare Workers** - Serverless 计算
- **Cloudflare KV** - 键值存储
- **JavaScript** - 核心逻辑
- **Telegram Bot API** - 通知推送

---

## 📜 许可证

[MIT License](LICENSE)

---

<div align="center">

### ⭐ Star this repo if it helps you!

Made with ❤️ by [Yeshenyue11](https://github.com/Yeshenyue11)

</div>
