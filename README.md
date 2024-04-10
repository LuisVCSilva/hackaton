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
      x: ['A', 'B', 'C', 'D'],
      y: [1, 2, 3, 4],
      type: 'scatter',
      mode: 'lines+markers',
      marker: { color: 'blue' },
    },
  ]}
  layout={{
    title: 'Line Chart Example',
    xaxis: { title: 'X Axis' },
    yaxis: { title: 'Y Axis' },
  }}
/>
