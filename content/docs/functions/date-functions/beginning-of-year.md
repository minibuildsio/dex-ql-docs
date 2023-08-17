---
title: "beginning_of_year"
draft: false
images: []
menu:
  docs:
    parent: "functions"
weight: 10
toc: true
---

Returns the beginning of the year of the provided date or now if no date is provided.

## Syntax

```
beginning_of_year([date])
```

## Parameters

| Name | Type | Required | Description |
| --- | --- | --- | --- |
| date | date/datetime | No | A date. Defaults to now if not provided. |

## Example

```
Steps
| project year = beginning_of_year(date)
```