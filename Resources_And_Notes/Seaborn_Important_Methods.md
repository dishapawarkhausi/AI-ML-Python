# Seaborn Library

This document provides a comprehensive list of methods available in Python's `seaborn` library, categorized by their respective functionalities.

## 1. Seaborn Plotting Functions (`seaborn`)

```python
import seaborn as sns
```

### a) Relational Plots
- `sns.scatterplot()` - Scatter plot
- `sns.lineplot()` - Line plot
- `sns.relplot()` - General relational plot

### b) Categorical Plots
- `sns.catplot()` - General categorical plot
- `sns.stripplot()` - Scatter plot for categorical data
- `sns.swarmplot()` - Categorical scatter plot with non-overlapping points
- `sns.boxplot()` - Box plot
- `sns.violinplot()` - Violin plot
- `sns.boxenplot()` - Enhanced box plot
- `sns.pointplot()` - Point plot
- `sns.barplot()` - Bar plot
- `sns.countplot()` - Count plot

### c) Distribution Plots
- `sns.histplot()` - Histogram
- `sns.kdeplot()` - Kernel Density Estimation (KDE) plot
- `sns.ecdfplot()` - Empirical Cumulative Distribution Function (ECDF) plot
- `sns.rugplot()` - Rug plot
- `sns.displot()` - General distribution plot

### d) Matrix Plots
- `sns.heatmap()` - Heatmap
- `sns.clustermap()` - Cluster map

### e) Regression Plots
- `sns.regplot()` - Regression plot
- `sns.lmplot()` - Linear regression plot

### f) Pair and Joint Plots
- `sns.pairplot()` - Pairwise relationships in dataset
- `sns.jointplot()` - Joint distribution plot

### g) Timeseries Plots
- `sns.tsplot()` - Time series plot (deprecated)
- `sns.lineplot()` - Line plot (recommended for time series)

## 2. Seaborn Styling Functions
- `sns.set()` - Set theme and style
- `sns.set_style()` - Set style only
- `sns.set_context()` - Set context for different environments
- `sns.set_palette()` - Set color palette
- `sns.color_palette()` - Retrieve color palettes
- `sns.dark_palette()` - Generate dark-themed palette
- `sns.light_palette()` - Generate light-themed palette
- `sns.diverging_palette()` - Generate diverging palette
- `sns.set_theme()` - Set complete theme

## 3. Seaborn Utility Functions
- `sns.load_dataset()` - Load example datasets
- `sns.get_dataset_names()` - List available datasets
- `sns.despine()` - Remove spines from plots
- `sns.move_legend()` - Move legend in plot
- `sns.objects()` - Access seaborn object-oriented interface (Seaborn v0.12+)

## 4. Seaborn Color Utilities
- `sns.husl_palette()` - Generate colors using HUSL space
- `sns.hls_palette()` - Generate colors using HLS space
- `sns.xkcd_palette()` - Colors using XKCD names
- `sns.crayon_palette()` - Colors using Crayola crayon names
- `sns.color_palette()` - Retrieve a color palette

## 5. Seaborn Figure-Level Functions
- `sns.FacetGrid()` - Create a grid of subplots
- `sns.PairGrid()` - Grid for pairwise relationships
- `sns.JointGrid()` - Grid for joint distribution plots

---

This document provides an organized overview of key methods in `seaborn`. For more details, refer to the [official documentation](https://seaborn.pydata.org/).
