# QRT Stock Return Prediction Project  
# QRT 股票收益预测项目

---

# English Version

## Project Overview

This project explores machine learning approaches for predicting stock returns using financial datasets.

We implement and compare three models:

- Baseline Model  
- XGBoost Model  
- Graph Neural Network (GNN)

The goal is to investigate whether incorporating **graph structure between stocks** can improve prediction performance.

---

## Project Pipeline

The workflow of this project is shown below:
Raw Financial Data
↓
Data Cleaning & Preprocessing
↓
Feature Engineering
↓
Baseline Model
↓
XGBoost Model
↓
Graph Construction
↓
Graph Neural Network
↓
Model Evaluation
---

## Model Results

Performance comparison:
Score Comparison

XGBoost                 
  ██████████████████████ 72  
Baseline Model           
  ███████████████████    69  
Graph Neural Network     
  █████████████████      67
| Model | Score |
|------|------|
| Baseline | 69 |
| XGBoost | **72** |
| Graph Neural Network | 67 |

XGBoost achieves the best performance in this experiment.  
The GNN model captures relationships between stocks but requires further tuning and improved graph construction.

---

## Methods

### Baseline Model

A baseline model is implemented to provide a reference performance level.

---

### XGBoost Model

XGBoost is a powerful gradient boosting model widely used for tabular data.

Advantages:

- Strong performance on structured datasets  
- Handles nonlinear relationships  
- Robust to missing values  

---

### Graph Neural Network

To model relationships between stocks, we construct a graph where:

- Nodes represent stocks  
- Edges represent relationships between stocks  

The GNN learns representations using both node features and graph structure.

---

## Tech Stack

Python  
Pandas  
NumPy  
Scikit-learn  
XGBoost  
PyTorch  
PyTorch Geometric  
Google Colab  

---

## Project Structure
QRT-project-for-public
├── baseline_model.ipynb
├── xgboost_model.ipynb
├── gnn_model.ipynb
└── README.md
---

# 中文说明

## 项目简介

本项目探索利用机器学习方法预测股票收益率。

项目实现并比较了三种模型：

- Baseline 基础模型  
- XGBoost 模型  
- Graph Neural Network（图神经网络）

研究目标是分析在金融预测任务中，引入**股票之间的关系网络结构**是否能够提升模型表现。

---

## 项目流程

项目整体流程如下：
原始金融数据
↓
数据清洗与预处理
↓
特征工程
↓
Baseline 模型
↓
XGBoost 模型
↓
股票关系图构建
↓
图神经网络（GNN）
↓
模型评估与结果比较
---

## 实验结果

模型表现对比：
模型得分对比

XGBoost                ██████████████████████ 72  
Baseline Model         ███████████████████    69  
Graph Neural Network   █████████████████      67
| 模型 | 得分 |
|------|------|
| Baseline | 69 |
| XGBoost | **72** |
| Graph Neural Network | 67 |

实验结果表明，在该数据集上 **XGBoost 模型表现最佳**。  
图神经网络虽然能够建模股票之间的关系结构，但仍需要进一步优化图构建方式和模型参数。

---

## 方法说明

### Baseline 模型

首先构建一个基础模型作为性能参考，用于评估后续复杂模型的改进效果。

---

### XGBoost 模型

XGBoost 是一种常用于结构化数据的梯度提升模型，在金融预测任务中表现稳定。

优势包括：

- 在表格数据上表现优秀  
- 能够建模非线性关系  
- 对缺失值具有较好的鲁棒性  

---

### 图神经网络（GNN）

为了刻画股票之间的关系，本项目构建股票关系图：

- 节点：股票  
- 边：股票之间的关系  

图神经网络能够同时利用**节点特征和图结构信息**进行学习，从而建模资产之间的相互影响。

---

## 技术栈

Python  
Pandas  
NumPy  
Scikit-learn  
XGBoost  
PyTorch  
PyTorch Geometric  
Google Colab  

---

## 项目总结

- 基于树模型的 **XGBoost 在金融表格数据上表现非常强**  
- 图神经网络提供了一种建模资产关系的新思路  
- 将图结构信息与传统机器学习模型结合可能是未来的重要研究方向

---

## 未来改进方向

可能的改进包括：

- 更合理的股票关系图构建方法  
- 更多金融因子特征工程  
- 模型超参数调优  
- 结合图嵌入与传统机器学习模型的混合方法
