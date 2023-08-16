---
title: "summarise"
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

Summarise using aggregation function and a group.

## Syntax

```
summarise Column = Aggregation(Expression)[, ...] by Column
```

## Parameters

| Name | Type | Required | Description |
| --- | --- | --- | --- |
| Column 1 | column | Yes | The new column to create. |
| Column 2 | column | Yes | The column to group by. |
| Aggregation | aggregation | Yes | The aggregation function such as `sum()`, `avg()`, etc. |
| Expression | expression | Depends on Aggregation | The expression to aggregate. |

#### Supported Aggregations 

| Aggregation | Description |
| --- | --- |
| count() | Count of the number of items |
| dcount(expression) | Count of the number of unique items |
| sum(expression) | Sum of the values of a given expression |
| avg(expression) | Average (mean) of the values of a given expression |
| min(expression) | Minimum of the values of a given expression |
| max(expression) | Maximum of the values of a given expression |


## Example

The following example will .

```
Steps
| project steps, month = beginning_of_month(date)
| summarise steps = sum(steps), distance = sum(0.00075 * steps) by month
```
