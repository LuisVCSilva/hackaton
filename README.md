---
datapackage:
  title: My own example
  description: This is not a template anymore
  licenses:
  - path: #http://opendatacommons.org/licenses/pddl/
    title: Open Data Commons Public Domain Dedication and License v1.0
  resources:
  - path: data.csv
    title: BTCxUSD
    name: btcusd
    format: csv
    schema:
      fields:
      - name: year
        type: date
      - name: co2
        type: number
---

Here's some text.

You can add as much text as you like.

The data files will be automatically displayed here.

We can add a chart:

<LineChart
  data="./data.csv"
  title="BTC - USD"
  xAxis="year"
  yAxis="value"
/>
