# Read: Class 14

1. **What are the key differences between Matplotlib, Seaborn, and Bokeh libraries in terms of their features and use cases? Provide an example of a specific visualization that is more suitable for each library.**

Matplotlib: 

Matplotlib is a basic plotting library in Python. It provides a wide variety of charts and graphs, but customization can sometimes be complex. It is good for basic visualizations and is highly customizable.

`import matplotlib.pyplot as plt`

`x = [1, 2, 3, 4, 5]`

`y = [2, 4, 6, 8, 10]`

`plt.plot(x, y)`

`plt.show()`

Seaborn: 

Seaborn is built on top of Matplotlib and provides a high-level interface for drawing attractive and informative statistical graphics. It simplifies the process of creating complex visualizations and is particularly good for statistical data visualization.

Bokeh: 

Bokeh is designed for interactive visualizations. It's suitable for creating interactive, web-ready plots that can be embedded into web applications.

2. **In the Seaborn library, what are the main functions to create relational, categorical, and distribution plots? Briefly explain the purpose of each type of plot and provide an example use case.**

Relational plots: `sns.relplot()`. These plots emphasize the relationship between two continuous variables.

`import seaborn as sns`

`tips = sns.load_dataset("tips")

`sns.relplot(x="total_bill", y="tip", data=tips, kind="scatter")`

Categorical plots: sns.catplot(). These plots show the distribution of a categorical variable across the levels of another categorical variable.

Distribution plots: sns.distplot(). These plots provide a univariate distribution of observations.

3. **Discuss the role of the Seaborn Cheat Sheet in a Python developer’s workflow. What are some key sections or elements featured in the cheat sheet that can help a developer quickly reference Seaborn functionalities?**

The Seaborn Cheat Sheet is a quick reference guide for Seaborn functionalities.
Key sections include:

Axes-level functions: These functions operate on a single subplot and are good for fine-tuning.

Figure-level functions: These functions create and manage entire figures.

Color palettes, themes, and contexts: Useful for customizing the visual appearance of plots.

Plot types and customizations: Quick reference for various plot types and their customization options.

The cheat sheet helps developers quickly find the right functions and settings for their visualization needs.

## `Things I want to know more about`
