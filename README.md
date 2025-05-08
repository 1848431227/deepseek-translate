# DeepSeek Office Translator

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
![Python Version](https://img.shields.io/badge/python-3.6%2B-blue)

[English](#english) | [中文](#中文)

<a name="english"></a>
## 🌍 DeepSeek Office Translator

A powerful tool that translates Microsoft Office documents (Word & Excel) while preserving their original formatting using the DeepSeek API.

### ✨ Features

- Supports both `.docx` and `.xlsx` file formats
- Preserves all original document formatting
- Supports 30+ languages including Chinese, English, Japanese, Korean, and more
- Smart batch processing for optimal translation efficiency
- Compatible with both openai-python 0.x and 1.x SDK versions

### 🚀 Installation

```bash
pip install -r requirements.txt
```

### 🔑 Configuration

Set your DeepSeek API key as an environment variable:

```bash
export DEEPSEEK_API_KEY="your-api-key"
```

Or modify the `API_KEY` variable in the script directly.

### 📖 Usage

```bash
python deepseek_translate.py [-h] -l TARGET_LANG file

# Example: Translate a Word document to English
python deepseek_translate.py document.docx -l en

# Example: Translate an Excel file to Japanese
python deepseek_translate.py spreadsheet.xlsx -l ja

# List all supported languages
python deepseek_translate.py --list-languages
```

### 🌐 Supported Languages

The tool supports translation between numerous languages, including but not limited to:
- Chinese (简体中文)
- English
- Japanese (日本語)
- Korean (한국어)
- French (Français)
- German (Deutsch)
- Spanish (Español)
- And many more...

Use `--list-languages` to see the complete list of supported languages and their codes.

---

<a name="中文"></a>
## 🌍 DeepSeek Office 文档翻译工具

一个强大的文档翻译工具，可以翻译 Microsoft Office 文档（Word 和 Excel），同时保持原有格式，基于 DeepSeek API。

### ✨ 特性

- 支持 `.docx` 和 `.xlsx` 文件格式
- 完整保留原文档格式
- 支持超过 30 种语言，包括中文、英文、日文、韩文等
- 智能分批处理，优化翻译效率
- 兼容 openai-python 0.x 和 1.x SDK 版本

### 🚀 安装

```bash
pip install -r requirements.txt
```

### 🔑 配置

将 DeepSeek API 密钥设置为环境变量：

```bash
export DEEPSEEK_API_KEY="your-api-key"
```

或直接在脚本中修改 `API_KEY` 变量。

### 📖 使用方法

```bash
python deepseek_translate.py [-h] -l 目标语言 文件

# 示例：将 Word 文档翻译成英文
python deepseek_translate.py document.docx -l en

# 示例：将 Excel 文件翻译成日文
python deepseek_translate.py spreadsheet.xlsx -l ja

# 列出所有支持的语言
python deepseek_translate.py --list-languages
```

### 🌐 支持的语言

该工具支持多种语言之间的互译，包括但不限于：
- 中文（简体中文）
- 英文
- 日文（日本語）
- 韩文（한국어）
- 法文（Français）
- 德文（Deutsch）
- 西班牙文（Español）
- 以及更多...

使用 `--list-languages` 查看完整的支持语言列表及其代码。

## 📄 License

MIT License 
