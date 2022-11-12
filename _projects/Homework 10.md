---
name: Homework 10
tools: [Python, HTML, vega-lite, Altair]
image: assets/pngs/hw10_thumbail.png
description: The homework 10 is the very first practice between Python, Jerkyll, and Vega-Lite !
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Homework 10 - Group 3



The idea of this analysis is visualizing the number of licenses which were issued from 1912 to 2022
## Figure 1

```python
  "Method" : Bar Chart
  "Encoding type" : Quantitative for counting | Temporal for Original Issue Date
```

<vegachart schema-url="{{ site.baseurl }}/assets/json/chart1.json" style="width: 100%"></vegachart>
 <center> Figure 1: The number of licenses were issued in 1912 to 2022. Chart created by Chien Nguyen </center>

<br />
According to the figure 1, we can see the the license system started recording the information from 1912, and the newest data was recorded in 2022.
We can also see that, in the figure one, the most licenses were issued between 1995 to 2000.

## Figure 2

```python
  "Method" : Scatter Plot
  "Scheme" : viridis
  "Variable Colored": Original Issue Date in Dataset
  "Encoding type" : Nominal for License Status and Type | Temporal for Original Issue Date
```

<vegachart schema-url="{{ site.baseurl }}/assets/json/scatter2.json" style="width: 100%"></vegachart>
 <center> Figure 2: The visualization of License Type and License Status - Chart created by Chien Nguyen </center>
<br />

In the figure 2, I applied Scatter plot to see the status of License Type based on License Status. As we can see that, all the license types have the status not renewed and active, and all this active licenses have the original issue year start from 2008 to now. The DETECTIVE BOARD license looks like got the most terminated after 2015.


## Figure 3

```python
  "Method" : Heat Map && Bar Chart 
  "Color" :  Base on number of Licenses were recorded
  "Encoding type" : Nominal for License Status and Type | Temporal for Original Issue Date
  "transform_filter": Brush
```

<vegachart schema-url="{{ site.baseurl }}/assets/json/dashboard_export.json" style="width: 100%"></vegachart>
<center> Figure 3: The interacting with user - Chart created by Chien Nguyen </center>
<br />
To take a look closer, I created the interactive charts that let everyone can interact with the license type and license status. The purpose of the figure 3 is you can see the number of license more clearly by looking to the history chart at the right side.
To use that, just drag the mouse on the heatmap on the left side, the data will automatically of date on the right chart. You can drag one box or many boxes in the heatmap and the result will show you on the left chart.


### Additional informations, click the buttons bellow to see the dataset and my code. Thanks for reading.

<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_bcubcg_fall2022/main/data/licenses_fall2022.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/cnguyen1411/cnguyen1411.github.io/blob/main/python_notebooks/HW10-Altair-Analysis.ipynb" text="The Analysis" %}
</div>

