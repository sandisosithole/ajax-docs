---
title: Series-Specific Properties
page_title: Series-Specific Properties | UI for ASP.NET AJAX Documentation
description: Series-Specific Properties
slug: chart/understanding-radchart-elements/series-specific-properties
tags: series-specific,properties
published: True
position: 10
---

# Series-Specific Properties



>caution  __RadChart__ has been replaced by[RadHtmlChart](http://www.telerik.com/products/aspnet-ajax/html-chart.aspx), Telerik's client-side charting component.	If you are considering __RadChart__ for new development, examine the[RadHtmlChart documentation](ffd58685-7423-4c50-9554-f92c70a75138)and[online demos](http://demos.telerik.com/aspnet-ajax/htmlchart/examples/overview/defaultcs.aspx)first to see if it will fit your development needs.	If you are already using __RadChart__ in your projects, you can migrate to __RadHtmlChart__ by following these articles:[Migrating Series](2f393f28-bc31-459c-92aa-c3599785f6cc),[Migrating Axes](3f1bea81-87b9-4324-b0d2-d13131031048),[Migrating Date Axes](93226130-bc3c-4c53-862a-f9e17b2eb7dd),[Migrating Databinding](d6c5e2f1-280c-4fb0-b5b0-2f507697511d),[Feature parity](010dc716-ce38-480b-9157-572e0f140169).	Support for __RadChart__ is discontinued as of __Q3 2014__ , but the control will remain in the assembly so it can still be used.	We encourage you to use __RadHtmlChart__ for new development.
>


The following are properties specific to the series appearance of specific [chart types]({%slug chart/understanding-radchart-types/radchart-types-overview%}).

## Bubble

The BubbleSize property is specific to the [Bubble]({%slug chart/understanding-radchart-types/bubble-charts%}) chart type and allows you to increase or decrease bubble size without distorting the shape.

## Lines and Splines

The LineSeriesAppearance property is specific to the [Line]({%slug chart/understanding-radchart-types/line-charts%}) and [Spline]({%slug chart/understanding-radchart-types/spline-charts%}) chart types.LineSeriesAppearance has a __Cap__ property that governs the appearance of a line terminating shape that occurs where at each data point (except the first).Valid __Cap__ values are __Flat__, __Square__, __Round__, __Triangle__, __NoAnchor__, __SquareAnchor__, __RoundAnchor__, __DiamondAnchor__, __ArrowAnchor__, __AnchorMask__ and __Custom__. LineSeriesAppearance also has sub properties for __Color__, __PenStyle__, __Visible__ and __Width__.

The PointMark is a shape that occurs at every data point, including the first.PointMarks are off by default but can be enabled using the Pointmark.Visible property. Use the Pointmark.Figure property to choose one of the predefined shapes. Other PointMark properties include __Border__, __Corners__, __Dimensions__, __FillStyle__, __RotationAngle__ and __Shadow__.
>caption 

![LineSeriesAppearance](images/radchart-understandingelements025.png)

The example above shows Series 1 in red where LineSeriesAppearance properties are:

* Cap = ArrowAnchor

* Color = Red

* PenStyle = Dash

* Width = 5

Series 2 show in blue has PointMark properties set as:

* Border.Color = 50, 0, 245, 100

* Border.Width = 1

*  Figure  = Star5

* Visible = True

* Dimensions.Height = 25px

* Dimensions.Width = 25px

* FillStyle.FillType = Solid

* FillStyle.MainColor = 90, 100, 254, 100

* Shadow.Blur = 1

* Shadow.Color = DimGray

* Shadow.Distance = 2

## Pie

The StartAngle property specifies degrees for the rotation of a pie. The default value and the starting position is 0°. Positive values of the StartAngle property will rotate the pie clockwise and negative - counterclockwise.
>caption 

![StartAngle Example](images/radchart-understandingelements026.png)



The DiameterScale property controls the ratio between the size of the plot area and the diameter of the chart. It effectively sets the size of the pie. In the example below, DiameterScale is set to 1, .75 (the default) and .5. 
>caption 

![DiameterScale Example](images/radchart-understandingelements027.png)





When true, the ShowLabelConnectors property visually ties the label with the corresponding pie slice.
>caption 

![ShowLabelConnectors](images/radchart-understandingelements028.png)



The ExplodePercent property defines the percentage of explosion of pie pieces. By default this is 20 percent.In the example below it is set to 50 percent:
>caption 

![ExplodePercent Example](images/radchart-understandingelements029.png)

The CenterXOffset and CenterYOffset properties specify the distance from the center of the plot area to the center of the pie in pixels. Use these two properties to position pie charts within the plot area.

