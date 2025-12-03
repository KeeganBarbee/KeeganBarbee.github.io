---
name: Homework 5 Jekyll Webpage
tools: [Python, Altair, vega-lite]
image: assets/pngs/Screenshot 2025-11-17 092542.png
description: This is Homework 5 which uses vega-lite and altair for interactive viz!
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---
# My Homework 5: Find the Data and the Analysis Below

<vegachart schema-url="{{ site.baseurl }}/assets/json/building_boxplot.json" style="width: 100%"></vegachart>

## Visualization 1 Description:
Essentially, what is being visualized here is the construction of all the buildings by year for every different agency and these agencies include different universities, colleges, departments, and much more. This graph can be helpful in identifying the inception of a certain agency based on its first building and also how present it is today based on where the IQR of the boxplot resides. However, everything should be taken with a grain of salt as many of these agencies still operate regardless of whether their buildings are old or not like the Historic Preservation Agency. There is a wide color scheme, so it is easier to differentiate the different agencies from each other. There is no set scheme but really just a vast array. I used boxplots for this graph because it visualizes the spread and median age of the buildings for an agency like mentioned before and this may provide insights into whether there may need to be some renovations for example. The x-axis encoding is of agencies, the y-axis is of the year they were constructed, and the color is of agencies as well. The reason for this is one quantitative and one qualitative variable for a boxplot. There were not a lot of transformations done other than removing some agencies that did not have a lot of buildings.

<vegachart schema-url="{{ site.baseurl }}/assets/json/building_chart.json" style="width: 100%"></vegachart>

## Visualization 2 Description: 
This graph is attempting to show the relationship between when a building was built and how big the building was. For this graph, there are some shortcomings. For example, when you change which agency is being shown, it automatically changes the scale of the graph, so that may be kind of confusing when interpreting it as you would always have to look back the axes. The filter allows users to change which agency they are looking at, so they can look at buildings for a specific group, almsot like a more in depth look at the first plot being able to see each data point and how big the building was along with when it was constructed. It is color-coded by building status. This is a useful encoding as it can tell you many things about whether a certain building is still operational or what is being newly built, so you see the overall progression of an agency over time. Also, be careful with that though as the color coding changes when you switch between agencies which is why the legend is turned on. The color coding is also better than most other ones because most categorical columns had many unique values and it would be too confusing. The interactivity makes it easier to focus on a single agency's building trends without being distracted by the clutter of points that make everything hard to interpret. So, overall it makes it clearer to understand the relationship between when a building was built and how big it is while also taking into consideration whether it is still operating.

<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_data/main/building_inventory.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://nbviewer.org/github/KeeganBarbee/KeeganBarbee.github.io/blob/main/Workbook.ipynb" text="The Analysis" %}
</div>
