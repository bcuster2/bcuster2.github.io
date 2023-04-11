---
name: Vega Lite plots, multiple ways
tools: [Python, HTML, vega-lite, Altair]
image: assets/pngs/cars.png
description: Vega-lite plots using differnet methods.
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Use Vega-lite in Many Ways in Jekyll

This project will show how to use vega-lite to make plots using different methods, and the vegachart tag from out plugins:

```
<vegachart schema-url="{{ site.baseurl }}/assets/json/cars.json" style="width: 100%"></vegachart>
```

## 1. Directly from vega-editor

<vegachart schema-url="{{ site.baseurl }}/assets/json/vega_editor_plot1.json" style="width: 100%"></vegachart>

<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://github.com/vega/vega/blob/main/docs/data/cars.json" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/jnaiman/online_cv_public/blob/main/python_notebooks/test_generate_plots.ipynb" text="The Analysis" %}
</div>

## 2. For real this time, vega-lite from vega-specs to JSON with Altair in Python.

Now here is an example of a side-by-side plot (not interactive though):

<vegachart schema-url="{{ site.baseurl }}/assets/json/license_dashboard.json" style="width: 100%"></vegachart>

I have added some interactivity with a 'altair.selection_interval' and 'tranform_filter':

<vegachart schema-url="{{ site.baseurl }}/assets/json/dashboard_of_licenses.json" style="width: 100%"></vegachart>

