---
title: "Introduction to PlanForge"
date: 2026-05-04
draft: false
tags: ["PlanForge", "Project"]
categories: ["Tech"]
ShowToc: true
TocOpen: true
---

# PlanForge: The Intelligent Developer Toolkit

## 🧠 Core Philosophy

PlanForge (formerly PasteKitLab) is a Chrome extension designed specifically for developers. Its core philosophy is: **Paste anything. We figure out the rest.**

While traditional developer tools follow a "Choose tool → Paste content → Process" workflow, PlanForge flips this model: **Paste content → PlanForge automatically selects the tool for you**. This small change results in a massive productivity boost.

## ✨ Why Choose PlanForge?

During development, we often find ourselves switching between multiple tool websites: JSON formatting, Base64 decoding, Cron expression parsing, DNS lookups, and more. PlanForge integrates all these tools into one place and uses an **Intelligent Content Detection Engine** to automatically recognize the type of content you paste, instantly displaying the corresponding utility.

*   **No Tab Switching**: All tools are integrated into a single extension.
*   **No Guessing**: Automatically identifies content types.
*   **Ctrl + V → Done**: A minimalist workflow.

## 🚀 Key Feature: Auto-Detection Engine

PlanForge analyzes your input and automatically activates the correct component:

| What you paste | What PlanForge does |
| :--- | :--- |
| `0 0 * * *` | Shows next 5 Cron execution times |
| `example.com` | DNS lookup (A / AAAA / CNAME) |
| `{ "a": 1 }` | JSON formatter & error locator |
| `MTIzNA==` | Auto-detects Base64 and decodes |
| `192.168.1.0/24` | Subnet calculator |
| `8.8.8.8` | IP information lookup |
| `1700000000` | Timestamp ⇄ Date conversion |
| Encoded text | Smart decode/encode panel |

## 🛠 Tech Stack

*   **Chrome Extension (Manifest V3)**
*   **React + TypeScript**
*   **DNS over HTTPS APIs**
*   **cron-parser**
*   **Pure Client-side Logic**: No backend server required, ensuring data privacy and security.

---

PlanForge is more than just a collection of tools; it is a **Content Detection Engine** designed to be the only developer tool you need to open when you're not sure which tool you need.
