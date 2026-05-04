---
title: "Introduction to Doc-Forge: AI-Powered Structured Document Engine"
date: 2026-05-04
draft: false
tags: ["Doc-Forge", "AI", "React"]
categories: ["Tech"]
ShowToc: true
TocOpen: true
---

# Doc-Forge: The Intelligent Technical Writing Assistant

## 🧠 Core Philosophy

**Doc-Forge** is an AI-assisted writing tool built on the Chrome Extension architecture. Its core philosophy is: **Transform unstructured ideas into logically rigorous professional documents**.

While traditional editors simply record text, Doc-Forge deeply participates in the creation process through its **Agent Pipeline**: from outline planning and content filling to multilingual polishing, achieving intelligent assistance throughout the entire workflow.

## ✨ Why Choose Doc-Forge?

*   **Structure First**: Enforces a tree-like hierarchy (H1-H4) for document management, ensuring clear logic in technical solutions.
*   **Agent Collaboration**: Supports custom AI workflows where different Prompts collaborate to complete complex tasks.
*   **Localization & Privacy**: Data is stored locally in `chrome.storage`, and API Keys are encrypted to ensure information security.
*   **Multi-platform Sync**: Built-in Git sync engine supports one-click push to GitHub, Gitee, GitLab, and other platforms.

## 🚀 Key Features

### 1. Intelligent Outline Generation
Simply input a goal (e.g., "Write a distributed lock implementation plan"), and the AI will automatically generate a detailed outline with multi-level chapters.

### 2. Three-Column Creation Interface
*   **Left Navigation**: Displays the document's tree structure in real-time, supporting drag-and-drop sorting and folding.
*   **Middle Editor**: Supports switching between Markdown source code and real-time preview, with built-in Token consumption statistics.
*   **Right AI Panel**: Provides quick commands like "Optimize," "Simplify," and "Expand," offering instant AI feedback.

### 3. Powerful Configuration Center
*   **Provider Config**: Supports mainstream LLM providers like Alibaba Cloud DashScope, OpenAI, DeepSeek, Claude, and Kimi.
*   **Prompt Engineering**: Allows users to customize Role definitions and Task descriptions to create their own exclusive writing experts.
*   **Agent Orchestration**: Chains multiple Prompts into a Pipeline for automated step-by-step execution.

### 4. Blog Metadata Management
Designed specifically for static blogs like Hugo/Jekyll, it allows direct configuration of `categories`, `tags`, `description`, and draft status within the editor.

## 🛠 Tech Stack

*   **Chrome Extension (Manifest V3)**
*   **React + Lucide Icons**
*   **Local Storage & Encryption**
*   **Markdown Rendering Engine**

---

Doc-Forge is dedicated to making technical writing as rigorous and efficient as coding, serving as a powerful assistant for every developer building their knowledge base.
