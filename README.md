# seaborn
**Seaborn** is a **Python data visualization library** built on top of **Matplotlib**. It’s designed to make **statistical graphics** more attractive, readable, and easier to create—especially when working with **pandas DataFrames**.

## What Seaborn Is Good At

* 📊 **Statistical visualizations** (distributions, relationships, categorical data)
* 🎨 **Beautiful default styles** (much nicer than plain Matplotlib)
* 🧠 **High-level plotting functions** (less code for complex plots)
* 🧩 **Tight integration with pandas**
* 🔢 Built-in support for **NumPy & SciPy**


## Installation


pip install seaborn


## Basic Usage


import seaborn as sns
import matplotlib.pyplot as plt

sns.set_theme()  # sets a nice default style


## Common Plot Types

### 1. Distribution plots


sns.histplot(data=df, x="age", kde=True)


* `histplot` – histogram
* `kdeplot` – density curve
* `boxplot`, `violinplot` – spread & outliers


### 2. Relationship plots


sns.scatterplot(data=df, x="height", y="weight", hue="gender")


* `scatterplot`
* `lineplot`
* `regplot` – regression line

### 3. Categorical plots

sns.barplot(data=df, x="day", y="sales")

* `barplot`
* `countplot`
* `stripplot`
* `swarmplot`

### 4. Matrix plots


sns.heatmap(corr_matrix, annot=True)

* `heatmap`
* `clustermap`

## Working with Built-in Datasets

Seaborn comes with sample datasets:

tips = sns.load_dataset("tips")
sns.boxplot(data=tips, x="day", y="total_bill")

Popular datasets:

* `tips`
* `iris`
* `titanic`
* `penguins`

## Styling & Themes

sns.set_style("whitegrid")
sns.set_palette("pastel")

Themes:

* `"darkgrid"`
* `"whitegrid"`
* `"dark"`
* `"white"`
* `"ticks"`


## Seaborn vs Matplotlib

| Feature           | Seaborn     | Matplotlib  |
| ----------------- | ----------- | ----------- |
| Ease of use       | ✅ High      | ❌ Lower     |
| Defaults          | ✅ Beautiful | ❌ Basic     |
| Statistical plots | ✅ Built-in  | ❌ Manual    |
| Custom control    | ⚠️ Medium   | ✅ Very High |

👉 **Seaborn = high-level & statistical**
👉 **Matplotlib = low-level & fully customizable**


## When to Use Seaborn

✔ Exploratory Data Analysis (EDA)
✔ Data science & ML projects
✔ Quick, publication-ready plots

