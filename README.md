# 🏗️ AI Domain Driven

AI领域驱动设计工具，支持DDD建模、聚合设计、限界上下文。

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.10+-blue?logo=python" />
  <img src="https://img.shields.io/badge/OpenAI-API-green?logo=openai" />
  <img src="https://img.shields.io/badge/License-MIT-yellow" />
</p>

## ✨ 特性

- 🏗️ 领域模型设计
- 📦 聚合设计
- 🔲 限界上下文设计
- 📢 领域事件生成
- 🗄️ 仓储实现生成
- 📊 领域复杂度分析

## 🚀 快速开始

```bash
pip install openai

python tools.py
```

## 📖 使用

```python
from ai_domain_driven import create_tools

tools = create_tools()

# 领域模型
domain = tools.design_domain_model("电商", "用户、商品、订单")

# 聚合设计
aggregate = tools.design_aggregate("订单", ["订单项", "支付"])

# 限界上下文
context = tools.design_bounded_context("电商", ["用户域", "商品域", "订单域"])

# 领域事件
event = tools.generate_domain_event("订单创建", {"orderId": "123"})

# 仓储实现
repo = tools.generate_repository("订单", "SQLAlchemy")

# 复杂度分析
complexity = tools.analyze_domain_complexity(domain_description)
```

## 📁 项目结构

```
ai-domain-driven/
├── tools.py       # DDD工具核心
└── README.md
```

## 📄 许可证

MIT License
