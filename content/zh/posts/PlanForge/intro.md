---
title: "PlanForge 项目介绍"
date: 2026-05-04
draft: false
tags: ["PlanForge", "Project"]
categories: ["Tech"]
ShowToc: true
TocOpen: true
---

# PlanForge：智能开发者工具集

## 🧠 核心理念

PlanForge（原 PasteKitLab）是一款专为开发者设计的 Chrome 扩展程序。它的核心理念是：**Paste anything. We figure out the rest.**（粘贴任何内容，剩下的交给我们。）

传统的开发者工具通常遵循“选择工具 → 粘贴内容 → 处理”的流程，而 PlanForge 颠覆了这一模式：**粘贴内容 → PlanForge 自动为你选择工具**。这种微小的改变带来了巨大的生产力提升。

## ✨ 为什么选择 PlanForge？

在开发过程中，我们经常需要在多个工具网站之间切换：JSON 格式化、Base64 解码、Cron 表达式解析、DNS 查询等。PlanForge 将这些工具整合在一起，并通过**智能内容检测引擎**自动识别你粘贴的内容类型，立即展示对应的实用工具。

*   **无需切换标签页**：所有工具集成在一个扩展中。
*   **无需猜测**：自动识别内容类型。
*   **Ctrl + V → 完成**：极简的操作流程。

## 🚀 核心功能：自动检测引擎

PlanForge 会分析你的输入并自动激活正确的组件：

| 粘贴内容 | PlanForge 的动作 |
| :--- | :--- |
| `0 0 * * *` | 显示接下来 5 次 Cron 执行时间 |
| `example.com` | DNS 查询 (A / AAAA / CNAME) |
| `{ "a": 1 }` | JSON 格式化与错误定位 |
| `MTIzNA==` | 自动检测 Base64 并解码 |
| `192.168.1.0/24` | 子网计算器 |
| `8.8.8.8` | IP 信息查询 |
| `1700000000` | 时间戳 ⇄ 日期转换 |
| 编码文本 | 智能解码/编码面板 |

## 🛠 技术栈

*   **Chrome Extension (Manifest V3)**
*   **React + TypeScript**
*   **DNS over HTTPS APIs**
*   **cron-parser**
*   **纯客户端逻辑**：无需后端服务器，确保数据隐私与安全。

---

PlanForge 不仅仅是一个工具集合，它是一个**内容检测引擎**，旨在成为当你不知道需要什么工具时，唯一需要打开的开发者工具。
