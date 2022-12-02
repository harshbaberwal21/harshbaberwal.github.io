---
name: Group 24 Final Project
tools: [Python, HTML, vega-lite]
image: assets/pngs/hc.png
description: This is a "showcase" project that uses vega-lite for interactive viz!
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---

# Hate Crime Cases Over the Years

Paragraph 1

## Bar Plot:
Paragraph 2

## Line Plot:
Paragraph 3



<vegachart schema-url="{{ site.baseurl }}/assets/json/group_24_final_project.json" style="width: 100%"></vegachart>

## About Selection: 
Paragraph 3

<div class="left">
{% include elements/button.html link="https://crime-data-explorer.fr.cloud.gov/pages/downloads" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/harshbaberwal21/harshbaberwal.github.io/blob/main/python_notebooks/group_24_final_project_part_2.ipynb" text="The Analysis" %}
</div>
