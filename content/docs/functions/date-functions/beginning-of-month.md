---
title: "beginning_of_month"
draft: false
images: []
menu:
  docs:
    parent: "functions"
weight: 20
toc: true
---

Returns the beginning of the month of the provided date or now if not date is provided.

## Syntax

```
beginning_of_month([date])
```

## Parameters

| Name | Type | Required | Description |
| --- | --- | --- | --- |
| date | date/datetime | No | A date. Defaults to now if not provided. |

## Example

```
Steps
| project month = beginning_of_month(date)
```