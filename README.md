---
datapackage:
  title: My own repo
  description: Testing from scratch repo
  licenses:
  - path: http://opendatacommons.org/licenses/pddl/
    title: Open Data Commons Public Domain Dedication and License v1.0
  resources:
  - path: data.csv
    title: BTC
    name: btc-volume
    format: csv
    schema:
      fields:
      - name: Date
        type: date
      - name: Volume
        type: number
---

Here are some plots

<LineChart
  data="data.csv"
  title="Bitcoin Data"
  xAxis="Date"
  yAxis="Volume"
/>

<PlotlyLineChart
  data={[
    {
      Volume: 902994450,
      Date: '01/10/2014'
    },
    {
      Volume: 659733360,
      Date: '01/11/2014'
    },
    {
      Volume: 1098811912,
      Date: '01/12/2014'
    },
    {
      Volume: 711518700,
      Date: '01/02/2015'
    }
  ]}
  xAxis="Date"
  yAxis="Volume"
/>
