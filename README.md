# Mino-Modeler（数策智联）

## 简介
Mino-Modeler 是一款集成多个国产 AI 大模型的数学建模辅助工具，旨在帮助用户高效完成数学建模任务。它能够自动完成题目拆解、数学计算、代码生成，并支持多模型讨论验证结果。

## 功能特点
- **题目拆解**：使用 SCNet 平台的大模型对题目进行分析和拆解，明确问题的关键点和要求。
- **数学计算**：调用讯飞星火 4.0 Ultra 模型进行数学公式的推导和计算，提供理论支持。
- **代码生成**：利用智谱 GLM-4V-Flash 模型根据分析和计算结果生成 Python 代码，减少手动编写工作。
- **多模型讨论**：综合多个模型的结果，验证逻辑一致性，确保最终答案的准确性和可靠性。

## 技术架构
- **SCNet 平台模型**：负责题目拆解，能够深入理解题目并提供详细分析。
- **讯飞星火 4.0 Ultra 模型**：负责数学计算部分，具备强大的数学推理能力。
- **智谱 GLM-4V-Flash 模型**：负责代码生成，能够根据给定的提示生成符合要求的 Python 代码。

## 使用方法

### 环境准备
确保你的环境中已安装以下依赖库：
```bash
pip install requests
```

### 配置信息
在代码中填写各个平台的 API 密钥和模型名称：
```python
# --- 全局变量（替换为你的API密钥）---
XF_APPID = "your_xf_appid"
XF_API_PASSWORD = "your_xf_api_password"
SCNET_API_KEY = "your_scnet_api_key"
SCNET_MODEL = "your_scnet_model"
ZHIPU_API_KEY = "your_zhipu_api_key"
```

### 运行程序
```bash
python math_modeling.py
```

### 输入题目
运行程序后，按照提示输入数学建模题目，程序将依次输出题目拆解、数学计算、代码生成和最终结论。

## 示例
输入题目：
```
设计一个优化模型，求解某物流公司运输成本最低路径。
```

程序输出：
```
【完整结果】
题目拆解：明确问题目标为寻找物流公司运输成本最低路径，涉及节点和边的权重表示运输成本。
数学计算：构建最短路径模型，使用 Dijkstra 算法求解最小运输成本。
代码生成：生成实现模型的 Python 代码，包括数据处理和结果可视化。
最终结论：综合所有结果，得出最优运输路径及其对应的成本。
```

## 项目地址
GitHub：[Omni-Modeler](https://github.com/iCurrer/Omni-Modeler)

## 联系方式
如有任何问题或建议，请联系：[iboy66lee@qq.com](mailto:iboy66lee@qq.com)
