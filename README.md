# 🔮 人生 K 线 (Life Destiny K-Line)

> **基于 AI 大模型和传统八字命理，将人生运势以 K 线图形式可视化展现。**

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/5lin/lifekline)

---

## ✨ 功能特点

1. **可视化运势**: 用股票 K 线图展示 1-100 岁的人生运势起伏，直观呈现人生"牛市"与"熊市"。
2. **专业命理体系**: 结合《滴天髓》《穷通宝鉴》，融合格局派、调候派、旺衰派。
3. **生命周期底盘**: 根据不同年龄阶段（童限、成长、青壮年、中老年）动态调整评分权重。
4. **AI 深度批断**: 生成性格、事业、财富、婚姻、健康等6大维度专业报告。
5. **多种导出**: 支持 JSON、HTML、PDF 格式，便于保存和分享。
6. **隐私保护**: API 调用在客户端进行，数据不经过服务器。

---

## 📝 使用方法

### 🔐 配置 API（必需）

本系统使用专业命理分析引擎，需要配置 AI API 才能获得准确分析。

**支持的 API：**
- OpenAI API（推荐 GPT-4）
- Anthropic Claude API（推荐 Opus/Sonnet）
- Google Gemini API（推荐 Pro）
- 其他兼容 OpenAI 格式的 API

**使用步骤：**

1. **填写八字信息** - 输入姓名、性别、出生年份、四柱干支、大运信息
2. **配置 API** - 填写模型名称、API Base URL、API Key
3. **生成分析** - 点击"生成人生K线"，等待 3-5 分钟
4. **查看结果** - 自动显示 K 线图和分析报告
5. **导出保存** - 支持导出 JSON、HTML、PDF 格式

### 💡 API 配置示例

**OpenAI API：**
- 模型名称：`gpt-4`
- API Base URL：`https://api.openai.com/v1`
- API Key：`sk-...`

**第三方代理（如有）：**
- 模型名称：`gemini-pro`
- API Base URL：`https://your-proxy.com/v1`
- API Key：`your-key`

### 📥 导入已有分析

如果你已有之前生成的 JSON 文件，可以直接导入：
- 点击"已有 JSON 文件？点击直接导入"
- 选择 JSON 文件即可立即查看分析结果

---

## 🚀 一键部署

### Vercel 部署（推荐）

点击下方按钮一键部署到 Vercel：

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/YOUR_USERNAME/lifekline)

### 本地运行

```bash
# 安装依赖
npm install

# 启动开发服务器
npm run dev

# 构建生产版本
npm run build
```

---

## 🛠️ 技术栈

- **前端框架**: React 19 + Vite
- **UI 样式**: TailwindCSS
- **图表库**: Recharts
- **AI 支持**: ChatGPT、Claude、Gemini 等任意 AI

---

## 📸 项目预览

![人生流年大运K线图](assets/1.png)
*(图1：人生流年大运 K 线走势图)*

![详细分析报告](assets/2.png)
*(图2：命理分析、币圈运势与风水建议)*

---

**免责声明**: 本项目仅供娱乐与文化研究，命运掌握在自己手中。切勿迷信，请理性看待分析结果。
