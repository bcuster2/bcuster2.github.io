---
name: Final Project
tools: [Python, HTML, vega-lite, altair]
image: assets/pngs/ContextViz1.png
description: This is the final project for Bennett Custer, Job Monita, and Sowmya Bhupatiraju
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---

# "Uncovering the Optimal Principal Components: The Power of PCA Scree Plots with Cumulative Variance for Correlated and Uncorrelated Variables"

Principal Component Analysis (PCA) is a widely used statistical method that reduces the dimensionality of a dataset by identifying the most important variables, known as principal components. One way to visualize the results of a PCA is by creating a scree plot.
A scree plot is a graphical tool that is commonly used in Principal Component Analysis (PCA) to help determine the optimal number of principal components to retain for subsequent analysis. A scree plot typically displays the eigenvalues of each principal component in descending order, along with a line representing the cumulative proportion of variance explained by the principal components.

In a scree plot, the eigenvalues are plotted on the y-axis and the principal components on the x-axis. A common practice is to plot both the eigenvalues and the cumulative variance explained by the principal components. The scree plot allows us to visualize the contribution of each principal component to the overall variance of the dataset.
We can use the cumulative variance explained to determine the optimal number of principal components to retain for further analysis. Generally, we want to retain enough principal components to capture at least 80-90% of the total variance in the data.

<vegachart schema-url="{{ site.baseurl }}/assets/json/Dashboard_primary.json" style="width: 100%"></vegachart>

This code seems to be generating a visualization of a rect plot for correlated variables, as part of a larger layered plot that includes a scree plot with cumulative variance.

The rect plot shows the explained variance for each principal component (PC), with the x-axis representing the PC component number and the y-axis representing the amount of explained variance. The color of each rectangle corresponds to the PC component number, with a tealblues color scheme used.The code also includes text annotations for each rectangle, displaying the amount of explained variance as a floating point number with 3 decimal places. Finally a line plot overlaid on the rect plot.
Additionally, the code includes a scree plot with cumulative variance, represented as both a line and point plot. This plot displays the cumulative amount of explained variance for each PC component, allowing users to identify the optimal number of PCs to include in their analysis.
Overall, this code is part of a dashboard that enables users to visualize the results of a principal component analysis for both correlated and uncorrelated variables. By using scree plots with cumulative variance, users can determine the optimal number of PCs to include in their analysis, helping to reduce the dimensionality of their data while retaining as much information as possible.

<vegachart schema-url="{{ site.baseurl }}/assets/json/dashboard_secondary.json" style="width: 100%"></vegachart>


In contrast, for uncorrelated variables, the eigenvalues and cumulative variance explained are expected to decline at a similar rate as for correlated variables. This is because uncorrelated variables already capture the maximum amount of information, and PCA does not need to remove any redundancy.

However, in this case, the scree plot will show a linear decline in both eigenvalues and cumulative variance explained!!!

This indicates that each principal component contributes equally to the overall variance of the data, and none of them are redundant.
A scree plot is a graphical tool that is commonly used in Principal Component Analysis (PCA) to help determine the optimal number of principal components to retain for subsequent analysis. 




Here's a few contextual visualizations that we found on the web (Sources for these visualizations are listed below):

<img src="https://juliasilge.com/blog/chicago-traffic-model/index_files/figure-html/unnamed-chunk-3-1.png" />

For this contextual visualization, the author was answering to the question "How have the number of crashes changed over time"[ Predicting], and the author has answered the question by showing a line chart of the number of traffic crashes per week over time withing of the city of Chicago. 

<img src="https://nycdsa-blog-files.s3.us-east-2.amazonaws.com/2018/02/default_map_view-1024x574.png" />
<!-- these are written in a combo of html and liquid --> 

For our second contextual visualization, the author has displayed an interactive Map of the city of New York, through it the author makes us explore by detail each the collision case of the city of New York, the programming language used in thus scenario is R.



Sources For Contextual Datasets:


“Predicting Injuries for Chicago Traffic Crashes.” Julia Silge, 4 Jan. 2021, https://juliasilge.com/blog/chicago-traffic-model/. 



“New York City Motor Vehicle Collision Data Visualization.” Data Science Blog, https://nycdatascience.com/blog/student-works/new-york-city-motor-vehicle-collision-data-visualization/. 


<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/bcuster2/bcuster2.github.io/main/_data/US_Accidents_small.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/Sowmya-BH/Sowmya-BH.github.io/blob/main/python_notebooks/Untitled15.ipynb" text="The Analysis" %}
</div>

