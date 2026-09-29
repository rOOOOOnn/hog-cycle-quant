# Hog Cycle Quant

## English

### Overview

Hog Cycle Quant is a quantitative research project focused on Chinese hog futures and livestock commodity cycles.

The objective is not to simply predict whether hog prices will rise or fall. Instead, the project aims to estimate the fundamental fair value of hog prices and identify potential mispricing between expected future spot prices and futures market prices.

Core idea:

```
Feed Cost
    ↓
Farming Profitability
    ↓
Breeding Sow Inventory
    ↓
Piglet Supply
    ↓
Market Hog Supply
    ↓
Spot Price
    ↓
Futures Pricing
```

The project will be developed in three stages:

---

## V1 — Hog Cycle Fundamental Model

Goal:
Understand whether biological supply cycles can explain future hog price movements.

Main variables:

- Breeding sow inventory
- Piglet prices
- Hog inventory
- Market weight
- Farming profitability
- Hog-to-grain ratio
- Spot hog prices

Research questions:

- How long does breeding sow inventory lead hog prices?
- Which indicators provide the earliest signals?
- Can supply cycles predict future spot prices?

Models:

- Correlation / lag analysis
- Linear models
- Logistic regression
- Gradient boosting models

---

## V2 — Futures Trading Framework

Goal:
Transform fundamental research into a futures trading strategy.

Additional information:

- Corn prices
- Soybean meal prices
- Feed costs
- Hog futures prices
- Basis
- Term structure
- Open interest
- Positioning data

Core framework:

Fair Value:

```
Expected Future Spot Price
```

Compared with:

```
Current Futures Price
```

Trading signal:

```
Fair Value - Futures Price
```

---

## V3 — Institutional Commodity Research Framework

Future extensions:

### Alternative Data

- News sentiment
- Farmer sentiment
- Industry reports
- Search trends

### Options Market

- Implied volatility
- Volatility skew
- Put/Call ratio
- Open interest distribution

### Global Market

- US Lean Hog futures
- Corn
- Soybeans
- Global livestock markets

### Regime Models

Potential methods:

- Hidden Markov Model
- Markov Switching Model
- Bayesian regime detection

---

## 中文

### 项目简介

Hog Cycle Quant 是一个针对中国生猪期货和农业商品周期的量化研究项目。

项目目标不是简单预测“猪价涨还是跌”，而是通过产业基本面建立未来现货价格估值模型，并比较：

```
未来现货合理价值
vs
当前期货市场价格
```

寻找期货市场可能存在的错误定价。

核心逻辑：

```
饲料成本
    ↓
养殖利润
    ↓
能繁母猪数量
    ↓
仔猪供应
    ↓
商品猪供应
    ↓
现货价格
    ↓
期货定价
```

---

# V1 — 生猪周期基本面模型

目标：

验证生猪产业周期是否具有预测未来价格的能力。

主要变量：

- 能繁母猪存栏
- 仔猪价格
- 生猪存栏
- 出栏体重
- 养殖利润
- 猪粮比
- 生猪现货价格

研究问题：

- 能繁母猪领先猪价多久？
- 哪些指标最早反映供需变化？
- 生猪周期是否可以量化预测？

模型：

- Lag analysis
- 线性模型
- Logistic Regression
- LightGBM / XGBoost

---

# V2 — 生猪期货交易框架

目标：

将基本面模型转化为期货交易策略。

加入：

- 玉米价格
- 豆粕价格
- 饲料成本
- LH期货价格
- 基差
- 期限结构
- 持仓量
- 多空持仓

核心：

预测：

```
未来现货合理价格
```

比较：

```
当前期货价格
```

交易信号：

```
Fair Value - Futures Price
```

---

# V3 — 机构级商品量化框架

未来扩展：

## 另类数据

- 新闻情绪
- 养殖户情绪
- 行业报告
- 搜索指数

## 期权市场

- 隐含波动率
- 波动率偏度
- Put/Call Ratio
- 持仓分布

## 全球市场

- 美国生猪期货
- 玉米
- 大豆
- 全球农产品市场

## 周期状态模型

方法：

- Hidden Markov Model
- Markov Switching Model
- Bayesian Regime Model
