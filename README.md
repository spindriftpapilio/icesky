# 冰霄 IceSky

面向AI安全测试的提示词注入综合工具，提供文本变换、Unicode隐写、多轮对话编辑，以及图像、音频、PDF、DOCX和富文本测试样本生成。

## 界面预览

![IceSky 工具界面](ui.png)

## 功能

| 模块 | 能力 |
| --- | --- |
| 文本变换 | 常见编码、古典密码、Unicode字形、大小写和格式转换，支持组合变换 |
| 解码与隐写 | 格式识别、文本解码、Emoji变体选择符隐写、不可见字符处理 |
| 多模态样本 | 编辑和生成图像、音频、PDF、DOCX与富文本载体 |
| 对话编辑 | 多轮消息编辑、材料与载荷组合、批量样本构造 |
| 文本扰动 | 字符映射、文本拆分、批量变异、噪声和Token压力样本 |
| 分析工具 | Token计数与可视化、异常Token、提示词注入分类与参考资料 |
| AI辅助 | 翻译与提示词变体生成，可用性取决于接口、模型和账户权限 |

### 部署

将整个目录上传到任何静态托管服务即可：

- GitHub Pages
- Cloudflare Pages
- Netlify
- Vercel
- AWS S3 + CloudFront
- 任何支持静态文件的Web服务器

## 项目结构

```
.
├── css/                    # 样式表
│   ├── components/         # 组件样式
│   ├── tools/              # 工具专用样式
│   └── vendor/             # 第三方CSS（FontAwesome）
├── js/                     # 前端逻辑
│   ├── app/                # 应用核心（导航、历史、命令）
│   ├── bundles/            # 打包的转换器模块
│   ├── config/             # 配置与元数据
│   ├── core/               # 核心功能（解码、隐写、工具注册）
│   ├── data/               # 数据文件（Emoji、Token、分类法）
│   ├── tools/              # 各工具实现
│   ├── utils/              # 工具函数
│   └── vendor/             # 第三方库（Vue.js）
```

## 工具列表

本应用包含以下工具：

- **Transform** - 文本编码转换（Base64、Hex、Unicode等）
- **Decode** - 自动识别和解码多种格式
- **ASCII Smuggler** - ASCII艺术与隐藏文本
- **Emoji** - Emoji变体选择符隐写
- **Bijection** - 自定义字符映射学习
- **Gibberish** - 噪声文本生成
- **Mutation** - 批量文本变异
- **Splitter** - 文本分割策略
- **Tokenizer** - Token分析与可视化
- **Tokenade** - Token压力测试
- **Sample Builder** - 多轮对话样本构造
- **Prompt Craft** - AI辅助提示词生成（需API）
- **Translate** - 多语言翻译（需API）
- **Injection Generator** - 提示词注入样本生成
- **Prompt Injection Taxonomy** - 注入技术分类参考
- **Jailbreak Library** - 越狱提示词库
- **Image Inject** - 图像载体生成
- **Audio Inject** - 音频载体生成
- **PDF Inject** - PDF载体生成
- **DOCX Inject** - DOCX载体生成
- **Rich Text Inject** - 富文本载体生成
- **Style Craft** - 文本样式转换

## 交流群

![IceSky交流群二维码](group.jpg)

## 免责声明

本工具仅供安全研究与教育用途。使用者应遵守相关法律法规和道德规范，对使用本工具产生的一切后果自行负责。

## Star 趋势

[![Stargazers over time](https://starchart.cc/spindriftpapilio/icesky.svg)](https://starchart.cc/spindriftpapilio/icesky)
