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

# Altair Plots

Here's our main visualization for our primary dataset:

<vegachart schema-url="{{ site.baseurl }}/assets/json/altair_mobility_dashboard.json" style="width: 100%"></vegachart>

Here's a few contextual visualizations that we found on the web (Sources for these visualizations are listed below):

<img src="https://juliasilge.com/blog/chicago-traffic-model/index_files/figure-html/unnamed-chunk-3-1.png" />

<img src="https://nycdsa-blog-files.s3.us-east-2.amazonaws.com/2018/02/default_map_view-1024x574.png" />
<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://github.com/vega/vega/blob/main/docs/data/cars.json" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/Sowmya-BH/Sowmya-BH.github.io/blob/main/python_notebooks/Untitled15.ipynb" text="The Analysis" %}
</div>

