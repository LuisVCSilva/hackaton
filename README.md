---
datapackage:
  title: Dataset Template
  description: A template for a dataset to publish on DataHub. Uses the Data Package metadata.
  licenses:
  - path: http://opendatacommons.org/licenses/pddl/
    title: Open Data Commons Public Domain Dedication and License v1.0
  resources:
  - path: data.csv
    title: BTCxUSD
    name: btcXusd
    format: csv
    schema:
      fields:
      - name: year
        type: date
      - name: open
        type: number
---

lorem ipsum

We can add a chart:

<LineChart
  data="./data.csv"
  title="BTCxUSD"
  xAxis="year"
  yAxis="volume"
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
