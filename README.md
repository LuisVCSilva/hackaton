---
datapackage:
  title: Bitcoin data!
  description: This is a template for publishing the data-set.  
  licenses:
  - path: http://opendatacommons.org/licenses/pddl/
    title: Open Data Commons Public Domain Dedication and License v1.0
  resources:
  - path: BTC-USD.csv
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


<LineChart
  data="BTC-USD.csv"
  title="Bitcoin Data"
  xAxis="Date"
  yAxis="Volume"
/>
