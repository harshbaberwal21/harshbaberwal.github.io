---
name: Vega Lite Example Project
tools: [Python, HTML, vega-lite]
image: assets/pngs/cars.png
description: This is a "showcase" project that uses vega-lite for interactive viz!
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---

# UFO Sightings Visualization

Below is a bar plot visualization of the number of ufo sightings in the USA by decade. This is bound interactively to another plot that visualizes a time series of the number of cases by month-year as a line plot. The bar plot is used from homework 9, while the other plot is novel. 

## Bar Plot:
For the bar plot, the x and y encodings are defined as decade and sum of number of sightings respectively. The color encoding is conditioned on the selection. The selection type used here is click that selects a single bar when clicked.

## Line Plot:
For the line plot the x and y encodings are the date (formatted to be month-year only) and sum of number of sightings respectively. The data for this visualization is transformed using the click selection.



<vegachart schema-url="{{ site.baseurl }}/assets/json/ufo_vis.json" style="width: 100%"></vegachart>

On selection of particular decade on the bar plot, the line plot gets truncated for the selected decade. To build these I prepared the data in python and then created the visualization using Altair.


<div class="left">
{% include elements/button.html link="https://github.com/UIUC-iSchool-DataViz/is445_bcubcg_fall2022/blob/main/data/ufo-scrubbed-geocoded-time-standardized-00.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/harshbaberwal21/harshbaberwal.github.io/blob/main/python_notebooks/UFO_Sightings_Viz.ipynb" text="The Analysis" %}
</div>
