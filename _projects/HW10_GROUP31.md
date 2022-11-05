---
name: Group32 homework 10
tools: [Python, HTML, vega-lite]
image: assets/pngs/plot1.png
description: Group32 homework 10
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---

# Homework 10

## plot1

<vegachart schema-url="{{ site.baseurl }}/assets/json/hw_10_plot1.json" style="width: 100%"></vegachart>

## Plot1 Description

This data visualization tried to find if the UFO sightings and intensity were related to environmental conditions like the moon phase, the weather, and the date.

## Plot1 Design choices - encodings

In this plot, the month-date variable is encoded as a temporal datatype, the precip_type is encoded as a nomial datatype.

## Plot1 Design choices - colormaps

This data visualization use three customized colors(reference to https://altair-viz.github.io/gallery/seattle_weather_interactive.html) to represent different weather condition for each data point. And apply light grey to the selected interval.

## Plot1 Transformations

In the data preprocessing, we replaced the Null value in the weather condition (precip_type) with 'Not recorded'。

## Plot2 Overlap with Homework #9

This data visualization is created based on the hw#9 plot 2 of the group member while adding more interactivity and variables.

# Plot 2

<vegachart schema-url="{{ site.baseurl }}/assets/json/hw_10_plot2.json" style="width: 100%"></vegachart>

## Plot2 Description

This data visualization tried to count the total number of UFO sightings for each state, embedded with the vega lite data set.

## Plot2 Design choices - encodings

The variables latitude, lontitude, and count(the sum of UFO sightings) are encoded as quantitative data type, and the state vairable is encoded as nomial data type.

## Plot2 Design choices - colormaps

We used orange to present the data point and use the circle size to indicate the quantity.

## Plot2 Transformations

The data has been processed to drop the null value and embedded with the vega-lite dataset for the US states' map.

## Plot2 overlap with Homework #9

This data visualization is created based on the hw#9 plot 1 of the group member while adding aggregate function.

# Interactivity (plot 1)

The interactivity includes select interval and create the barplot based on the selected data could show the relationships between UFO sightings and weather more clearly.

<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_bcubcg_fall2022/main/data/bfro_reports_fall2022.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/WeiruSun/WeiruSun.github.io/tree/main/python_notebooks/IS445 HW10 group 32.ipynb" text="The Analysis" %}
</div>
