---
title: "summarise"
draft: false
images: []
menu:
  docs:
    parent: "tabular-expressions"
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

The following example will create a table of total steps and total distance by month.

```
Steps
| project steps, month = beginning_of_month(date)
| summarise steps = sum(steps), distance = sum(0.00075 * steps) by month
```
