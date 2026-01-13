# Google MyActivity Keyword Cleaner

[中文版本](./README_zh.md)

A modern Tampermonkey UserScript designed for deep cleaning of Google MyActivity history. It uses an intelligent context-matching engine to precisely delete entries containing specific keywords.

## 🌟 Key Features

- **Premium UI**: Sleek **Glassmorphism** design, compact and refined (240px width).
- **Aggressive Matching Engine**:
  - **Deep Context Scan**: Automatically checks up to 15 levels of parent containers—finds matches even when keywords aren't directly in the button label.
  - **Multi-dimensional Detection**: Supports `aria-label`, visible text, `title` attributes, and `role="button"` elements.
  - **Character Normalization**: Automatically unifies full-width/half-width symbols (e.g., `：` vs `:`) and ignores case.
- **Smart Error Handling**: Automatically detects consecutive failures (e.g., Captchas) and auto-stops after 3 attempts to ensure safety.
- **I18n Support**: Automatically detects page language and toggles between English and Chinese.
- **Real-time Stats**: Track session-specific and total lifetime deletions.
- **Fully Automated**: Auto-scrolls to load more items and handles confirmation dialogs automatically.

## 🚀 Installation

1.  Install the [Tampermonkey](https://www.tampermonkey.net/) extension.
2.  Copy the source code from [GoogleMyActivityKeywordCleaner.user.js](./GoogleMyActivityKeywordCleaner.user.js).
3.  Create a new script in Tampermonkey, paste the code, and Save.
4.  Navigate to your [Google MyActivity](https://myactivity.google.com/) page.

## 📖 Usage

1.  Find the **Cleaner Configuration** panel at the bottom right of the page.
2.  Enter the keyword you wish to target (e.g., `提示 Role:`).
3.  Click **Start Cleaning**. The script will begin its automated scan and deletion process.
4.  To stop, click the same button (now labeled **Stop**).

## 🛡️ Disclaimer

Use at your own risk. This script performs actual deletions on your Google account records. It is recommended to test with specific keywords before wide-scale cleaning.

---
**Version**: 1.3.20260113.0955
