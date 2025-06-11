Abhishek mishra.

-> Seaborn is a Python data visualization library built on top of Matplotlib.
It provides a high-level interface for creating attractive and informative statistical graphics with just a few lines of code.

Main features:
Beautiful default styles
Simplifies complex plots
Built-in support for pandas DataFrames
Statistical visualization (regression plots, distributions, heatmaps, etc.)

Q. Why use Seaborn?
Much simpler syntax compared to Matplotlib for common plots.
Easy to plot relationships between multiple variables.
Automatically handles DataFrame columns, legends, and color palettes.
Produces publication-quality graphics by default.

**Seaborn Cheatsheet**
import seaborn as sns
import matplotlib.pyplot as plt
import pandas as pd

Optional: Load sample dataset

df = sns.load_dataset("tips")


 Basic Plots

 sns.scatterplot(data=df, x="total_bill", y="tip", hue="sex")
plt.show()


Line plot

sns.lineplot(data=df, x="total_bill", y="tip")
plt.show()

Bar plot
sns.barplot(data=df, x="day", y="total_bill")
plt.show()

Count Plot (for counts of categories)

sns.countplot(data=df, x="day")
plt.show()


Box Plot

sns.boxplot(data=df, x="day", y="total_bill")
plt.show()

Violin Plot
sns.violinplot(data=df, x="day", y="total_bill", hue="sex", split=True)
plt.show()

Strip Plot (scatter over categories)
sns.stripplot(data=df, x="day", y="total_bill", jitter=True)
plt.show()

Swarm Plot (non-overlapping scatter)
sns.swarmplot(data=df, x="day", y="total_bill")
plt.show()


