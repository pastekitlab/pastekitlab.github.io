---
title: "PlanForge User Guide"
date: 2026-05-04
draft: false
tags: ["PlanForge", "Tutorial"]
categories: ["Tech"]
ShowToc: true
TocOpen: true
---

# PlanForge User Guide

## 📦 Installation & Setup

### Development Environment Installation

1.  **Clone the Repository**:
    ```bash
    git clone https://github.com/pastekitlab/pastekitlab.git
    cd pastekitlab
    ```
2.  **Install Dependencies and Build**:
    ```bash
    npm install
    npm run build
    ```
3.  **Load the Extension**:
    *   Enter `chrome://extensions/` in your Chrome browser's address bar.
    *   Enable "Developer mode" in the top right corner.
    *   Click "Load unpacked" and select the `dist` folder in the project root directory.

### HTTPS Development Environment

This project includes a complete HTTPS development environment for testing secure connections and certificate handling:

```bash
# 1. Set up local SSL certificates (first time only)
./scripts/setup-local-ssl.sh

# 2. Start the HTTPS test environment
./start-https-test.sh

# 3. Visit https://localhost:8443
```

## 🧩 Built-in Components Explained

### 🕒 Cron Viewer
*   **Function**: Parses cron expressions and shows the next 5 execution times.
*   **Usage**: Simply paste an expression like `0 0 * * *`.

### 🌐 DNS Resolver
*   **Function**: Automatically detects domains and resolves A / AAAA / CNAME records via DNS over HTTPS.
*   **Usage**: Paste a domain name (e.g., `example.com`).

### 🔐 Encode / Decode Lab
*   **Supported Formats**: Base64, URL Encode, Hex, Unicode, ASCII Bytes, UTF-8 Bytes.
*   **Smart Logic**: If the content is encoded, it will automatically attempt to decode it; otherwise, it defaults to Base64 encoding.

### 🧾 JSON Tool
*   **Function**: Format or Minify JSON.
*   **Error Location**: Provides a smart error pointer that displays characters around the error location for quick debugging.

### 🌍 IP & Subnet Tool
*   **Function**: Query detailed IP information, get your public IP, and perform CIDR subnet calculations (start IP, end IP, host count).

### ⏱ Timestamp Tool
*   **Function**: Automatically detects timestamps or date strings and performs bidirectional conversion, while also displaying the current time.

## 💡 Best Practices

*   **One-Click Paste**: After copying content from anywhere, simply paste it into the extension's input box to trigger detection.
*   **History Panel**: (Coming soon) Use the history panel to review previous conversion results.
*   **Privacy Protection**: All processing is done locally on the client side; no data is uploaded to any server.
