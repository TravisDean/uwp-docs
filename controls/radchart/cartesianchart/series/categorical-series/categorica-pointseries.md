---
title: Categorical Stroked Series Class
page_title: Categorical Stroked Series Class
description: Categorical Stroked Series Class
slug: radchart-series-cartesianchart-series-categoricalseries-categoricalstrokedseriesclass
tags: categorical,stroked,series,class
published: True
position: 1
---

# Categorical Stroked Series Class



The **CategoricalStrokedSeries** class is a base class for all series that are visually represented by data points connected with strokes.


## Properties

>**CategoricalStrokedSeries** class inherits from the **CategoricalSeries** class -
[See the inherited properties]({%slug radchart-series-cartesianchart-series-categorical-categoricalseriesclass%}).


* **Stroke** (Brush): Gets or setst the **Brush** instance that defines the stroke of the line used to present the series.


* **StrokeThickness** (double): Gets or sets the thickness of the line used to present the series.

---
title: Point Series
page_title: Point Series
description: Point Series
slug: radchart-cartesianchart-series-categoricalseries-pointseries
tags: point,series
published: True
position: 6
---

# Point Series

## Overview

PointSeries represents its DataPoints as Ellipses.

![Point Series Overview](images/PointSeriesOverview.png)

## Properties

>**PointSeries** class inherits from the **CategoricalSeriesBase** class -
[See the inherited properties]({%slug radchart-series-cartesianchart-series-categorical-categoricalseriesclass%}).

* **PointSize**: Gets or sets the Size of the points. This property will be ignored if PointTemplate property is set.
* **LegendTitleBinding**: Gets or sets the binding that will be used by any attached legend to display legend item title.
* **PaletteMode**: Gets or sets the target type to that chart palette will be applied to. The available types are:
	* **Series**: Applies the palette per series.
	* **DataPoint**: Applies the palette per points.

## Example

Here's an example of how to create a **RadCartesianChart** with**PointSeries**.

	<telerikChart:RadCartesianChart>
	    <telerikChart:RadCartesianChart.HorizontalAxis>
	        <telerikChart:CategoricalAxis/>
	    </telerikChart:RadCartesianChart.HorizontalAxis>
	    <telerikChart:RadCartesianChart.VerticalAxis>
	        <telerikChart:LinearAxis/>
	    </telerikChart:RadCartesianChart.VerticalAxis>
	
	    <telerikChart:PointSeries  PointSize="15,15">
	        <telerikCharting:CategoricalDataPoint Category="first" Value="10"/>
	        <telerikCharting:CategoricalDataPoint Category="second" Value="20"/>
	        <telerikCharting:CategoricalDataPoint Category="third" Value="30"/>
	        <telerikCharting:CategoricalDataPoint Category="fourth" Value="15"/>
	    </telerikChart:PointSeries>
	</telerikChart:RadCartesianChart>