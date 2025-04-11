# AntiScam-Callguard🛡️

一款完全本地运行的安卓应用，实时分析通话内容并识别诈骗风险。

## 功能特性

- 📞 **自动监听来电**：通话时自动启动录音  
- 🔒 **隐私保护**：所有数据处理均在本地完成  
- 🚨 **实时提醒**：检测到风险关键词时震动并弹窗  
- 📂 **通话历史**：查看录音、文字内容和检测结果  

## 技术栈

- **前端**: Android (Kotlin)  
- **语音识别**: [Vosk离线引擎](https://alphacephei.com/vosk/)  
- **AI模型**: TensorFlow Lite (预训练诈骗关键词分类模型)  
- **本地存储**: SQLite + 文件系统  

## 项目目录结构示意

AntiFraudCallAssistant/  
├── .github/                  # GitHub 配置
│   └── ISSUE_TEMPLATE/       # Issue 模板
│       ├── bug_report.md
│       └── feature_request.md
├── app/                      # Android 前端代码
│   ├── src/
│   │   └── main/
│   │       ├── java/        # Kotlin/Java 代码
│   │       ├── res/         # 资源文件（布局、图片）
│   │       └── assets/      # 模型文件（.tflite、Vosk 模型）
│   └── build.gradle
├── model/                    # 模型训练代码（可选）
│   ├── train.py             # TensorFlow Lite 模型训练脚本
│   └── dataset/             # 训练数据
├── docs/                     # 所有文档
│   ├── requirements.md      # 需求文档
│   ├── api.md               # API 接口说明
│   └── user_guide.md        # 用户手册
├── scripts/                  # 辅助脚本
│   └── deploy.sh            # 自动化部署脚本（可选）
├── LICENSE                  # 开源协议（MIT）
├── README.md                # 项目总览
└── .gitignore               # Git 忽略规则（Android 模板）

## 快速开始

### 环境要求

- Android Studio 2022+  
- Android 8.0及以上设备  

### 安装步骤
