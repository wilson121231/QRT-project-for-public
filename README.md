# Stock Return Prediction using Machine Learning and Graph Neural Networks

## Project Overview

This project aims to predict stock returns using machine learning models.  
The workflow includes data preprocessing, feature engineering, baseline model construction, and advanced modeling using Graph Neural Networks (GNN).

We compare the performance of classical machine learning models and graph-based deep learning models to analyze their effectiveness in financial prediction tasks.

---

## Methodology

The project consists of three main modeling approaches:

### 1. Baseline Model

A simple baseline model is implemented to establish a performance reference.

Baseline score: **69**

---

### 2. XGBoost Model

XGBoost is used as the primary machine learning model for structured financial data.

Reasons for using XGBoost:

- Strong performance on tabular datasets
- Robust to missing values
- Effective for nonlinear feature interactions

Model score: **72**

This model achieves the best performance among the tested approaches.

---

### 3. Graph Neural Network (GNN)

To capture relationships between stocks, we construct a stock graph and apply a Graph Neural Network model.

Graph structure:

- Nodes: stocks
- Edges: relationships between stocks (e.g., similarity or correlation)

The GNN model integrates both node features and graph structure to learn stock representations.

Model score: **67**

Although the GNN model does not outperform XGBoost in this experiment, it demonstrates the potential of graph-based learning for financial prediction tasks.

---

## Results

| Model | Score |
|------|------|
| Baseline Model | 69 |
| XGBoost | **72** |
| Graph Neural Network | 67 |

---

## Tech Stack

- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- XGBoost  
- PyTorch  
- PyTorch Geometric  
- Google Colab  

---

## Project Structure

---

# 中文说明

## 项目简介

本项目旨在利用机器学习方法预测股票收益率。  
项目通过构建不同模型并进行对比分析，探索传统机器学习方法与图神经网络在金融预测任务中的表现。

项目实现了三种模型：

- Baseline 基础模型
- XGBoost 模型
- Graph Neural Network（图神经网络）

---

## 实验结果

| 模型 | 得分 |
|------|------|
| Baseline | 69 |
| XGBoost | **72** |
| GNN | 67 |

实验结果表明，在该数据集上 **XGBoost 模型表现最佳**。  
图神经网络模型虽然未超过 XGBoost，但能够捕捉股票之间的关系信息，在金融预测任务中具有潜在价值。

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
