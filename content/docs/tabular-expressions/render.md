---
title: "render"
draft: false
images: []
menu:
  docs:
    parent: "tabular-expressions"
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
