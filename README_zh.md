# Google MyActivity Keyword Cleaner (谷歌活动记录关键词清理器)

[English Version](./README.md)

一个现代化的油猴脚本 (Tampermonkey UserScript)，专为深度清理 Google 我的活动 (MyActivity) 历史记录而设计。它能够通过智能的上下文匹配引擎，精准删除包含特定关键词的活动条目。

## 🌟 核心特性

- **极致美学 (Premium UI)**：采用 **Glassmorphism (磨砂玻璃)** 设计风格，界面精致、纤细且不占空间（240px 宽度）。
- **智能匹配引擎 (Aggressive Matching)**：
  - **深度上下文扫描**：自动向上查找 15 层父容器，即使关键词不在按钮标签上也能精准识别。
  - **多维检测**：支持 `aria-label`、可见文本、标题 (`title`) 以及 `role="button"` 等多种元素。
  - **字符归口**：全角/半角符号（如 `：` vs `:`）自动统一，大小写自动忽略。
- **智能错误处理 (Smart Error Handling)**：自动监控连续失败次数（如遇到验证码或 UI 变化），连续 3 次失败将自动熔断停止，确保账户安全。
- **国际化支持 (i18n)**：自动识别页面语言，支持中文和英文界面切换。
- **实时统计**：清晰展示本次会话及累计清理的总数。
- **自动化操作**：自动滚动页面加载更多，自动触发清理确认，完全解放双手。

## 🚀 安装步骤

1.  安装脚本管理器 [Tampermonkey](https://www.tampermonkey.net/)。
2.  点击 [GoogleMyActivityKeywordCleaner.user.js](./GoogleMyActivityKeywordCleaner.user.js) 查看源代码并复制。
3.  在 Tampermonkey 中新建脚本，粘贴内容并保存。
4.  访问 [Google 我的活动 (MyActivity)](https://myactivity.google.com/) 页面。

## 📖 使用说明

1.  页面右下角会显示**清理器配置**面板。
2.  在输入框中输入你想要清理的关键词（例如 `提示 Role:`）。
3.  点击 **开始清理**，脚本将自动扫描并执行删除。
4.  需要停止时，点击原按钮（此时显示为**停止**）即可。

## 🛡️ 免责声明

请谨慎使用。此脚本会真实删除您的 Google 账户记录。在执行大规模清理前，建议先使用非关键词进行测试。

---
**版本号**: 1.3.20260113.0955
