---
title: "render"
date: 2020-10-06T08:48:57+00:00
lastmod: 2020-10-06T08:48:57+00:00
draft: false
images: []
menu:
  docs:
    parent: "tabluar-expressions"
weight: 100
toc: true
---

Render the input table as a visualisation for example a chart.

## Syntax

```
render Type [with PropertyName = PropertyValue, ...]
```

## Parameters

| Name | Type | Required | Description |
| --- | --- | --- | --- |
| Type | enum | Yes | The type of visualisation linechart, barchart, or table. |
| PropertyName | name | No | The name of a property to pass to the render e.g. title. |
| PropertyValue | string or int | No | The value of the property. |

## Example

The following example will render the input table as a line chart with a title of "Step Chart".

```
Steps
| render linechart with title = "Step Chart"
```
