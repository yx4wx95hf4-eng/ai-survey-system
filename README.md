# 企业AI应用与技能需求调查问卷系统

在线问卷调查系统，Flask + SQLite 后端，支持云端独立部署。

## 功能特性

- 📋 问卷填报（5部分，含B1智能跳题逻辑）
- 📊 数据看板（Chart.js 可视化统计）
- 📈 趋势分析（28天趋势图）
- 🔀 交叉分析（行业×AI率、规模×AI率）
- 📥 CSV 数据导出
- 🔒 IP 提交限制 + 速率限制
- ⏱️ 问卷开关 + 时间窗口控制
- 💾 前端草稿自动保存

## 文件结构

```
survey-system/
├── server.py              # Flask 后端 (v2.7)
├── requirements.txt       # Python 依赖
├── render.yaml            # Render.com 部署配置
├── static/
│   ├── index.html         # 问卷前端
│   └── admin.html         # 管理后台
└── .gitignore
```

## 管理密码

```
admin2026
```

## 部署方式

### 方式一：本地运行

```bash
pip install flask
python server.py
# 问卷: http://localhost:8080/
# 后台: http://localhost:8080/admin
```

### 方式二：云端部署 (推荐)

**一键部署到 Render.com：**

[![Deploy to Render](https://render.com/images/deploy-to-render-button.svg)](https://render.com/deploy)

部署后获得公开 URL，无需电脑在线，手机/电脑均可访问。
