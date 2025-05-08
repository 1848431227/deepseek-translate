# deepseek-translate

> **一键把 Word / Excel 文档完整翻译成另一种语言，排版、样式、公式、VBA 统统不动！**  
> 基于 [DeepSeek](https://deepseek.com) 大模型 · 支持 `openai-python` **0.x** / **1.x** 双版本 SDK

---

## 功能亮点

|  | 功能 |
|---|---|
| 📄 **双格式支持** | 直接翻译 `.docx`（Word）和 `.xlsx`（Excel）文件 |
| 🎨 **保持原始排版** | 字体、段落样式、文本颜色、合并单元格、公式、VBA 宏全部保留 |
| 🧩 **SDK 自动兼容** | 无需改代码，即可在旧版 `openai`（0.x）或新版 `openai`（≥1.x）环境下运行 |
| 🔄 **批量分段翻译** | 自动切分段落 / 单元格，智能分批避免上下文长度溢出 |
| 🛡 **键名兜底容错** | 即使模型偶发返回奇怪 JSON 字段也能自动修复 |
| 🌍 **多语言** | 内置 30+ 语言代码映射，可用别名如 `cn`→`zh`、`eng`→`en` |
| 🛠 **CLI 即开即用** | `deepseek_translate.py <文件> -l <目标语言>`，省心省力 |

---

## 快速开始

### 1. 安装依赖

```bash
# Python ≥3.9
pip install -r requirements.txt
# 或手动安装
pip install openai~=1.14.0 python-docx openpyxl tiktoken tqdm
## 2. 配置 DeepSeek API Key

```bash
export DEEPSEEK_API_KEY="sk-xxxxxxxxxxxxxxxx"

## 3. 翻译文件

```bash
# 将 test.docx 翻译成日语
python deepseek_translate.py test.docx -l ja

# 将 data.xlsx 翻译成繁体中文
python deepseek_translate.py data.xlsx -l zh-tw

| 代码    | 语言               | 代码 | 语言            |
| ----- | ---------------- | -- | ------------- |
| zh    | 简体中文             | ja | 日本語           |
| zh-tw | 繁體中文             | ko | 한국어           |
| en    | English          | fr | Français      |
| de    | Deutsch          | es | Español       |
| it    | Italiano         | pt | Português     |
| ru    | Русский          | nl | Nederlands    |
| pl    | Polski           | tr | Türkçe        |
| vi    | Tiếng Việt       | th | ไทย           |
| id    | Bahasa Indonesia | ms | Bahasa Melayu |
| hi    | हिन्दी           | bn | বাংলা         |
| ta    | தமிழ்            | ar | العربية       |
| fa    | فارسی            | he | עברית         |
| sw    | Kiswahili        | el | Ελληνικά      |
| cs    | Čeština          | hu | Magyar        |
| ro    | Română           | uk | Українська    |
| fi    | Suomi            | sv | Svenska       |
| da    | Dansk            | no | Norsk         |
