---
title: "PlanForge 使用指南"
date: 2026-05-04
draft: false
tags: ["PlanForge", "Tutorial"]
categories: ["Tech"]
ShowToc: true
TocOpen: true
---

# PlanForge 使用指南

## 📦 安装与启动

### 开发环境安装

1.  **克隆仓库**：
    ```bash
    git clone https://github.com/pastekitlab/pastekitlab.git
    cd pastekitlab
    ```
2.  **安装依赖并构建**：
    ```bash
    npm install
    npm run build
    ```
3.  **加载扩展**：
    *   在 Chrome 浏览器地址栏输入 `chrome://extensions/`。
    *   开启右上角的“开发者模式”。
    *   点击“加载已解压的扩展程序”，选择项目根目录下的 `dist` 文件夹。

### HTTPS 开发环境

本项目包含完整的 HTTPS 开发环境，用于测试安全连接和证书处理：

```bash
# 1. 设置本地 SSL 证书（首次运行）
./scripts/setup-local-ssl.sh

# 2. 启动 HTTPS 测试环境
./start-https-test.sh

# 3. 访问 https://localhost:8443
```

## 🧩 内置组件详解

### 🕒 Cron 表达式查看器
*   **功能**：解析 Cron 表达式并显示接下来 5 次的执行时间。
*   **用法**：直接粘贴如 `0 0 * * *` 的表达式。

### 🌐 DNS 解析器
*   **功能**：自动检测域名并通过 DNS over HTTPS 解析 A / AAAA / CNAME 记录。
*   **用法**：粘贴域名（如 `example.com`）。

### 🔐 编码/解码实验室
*   **支持格式**：Base64, URL Encode, Hex, Unicode, ASCII Bytes, UTF-8 Bytes。
*   **智能逻辑**：如果内容是编码后的，会自动尝试解码；否则默认进行 Base64 编码。

### 🧾 JSON 工具
*   **功能**：格式化或压缩 JSON。
*   **错误定位**：提供智能错误指针，显示错误位置周围的字符，方便快速调试。

### 🌍 IP 与子网工具
*   **功能**：查询 IP 详细信息、获取本机公网 IP、CIDR 子网计算（起始 IP、结束 IP、主机数）。

### ⏱ 时间戳工具
*   **功能**：自动检测时间戳或日期字符串，并进行双向转换，同时显示当前时间。

## 💡 最佳实践

*   **一键粘贴**：在任何地方复制内容后，直接在扩展中输入框粘贴即可触发检测。
*   **历史记录**：(即将推出) 利用历史面板回顾之前的转换结果。
*   **隐私保护**：所有处理均在本地客户端完成，数据不会上传至任何服务器。
