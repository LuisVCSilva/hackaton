![image](https://github.com/LuisVCSilva/hackaton/assets/23017780/bbfd07ad-0ce2-4d41-b6cd-80156dc5f043)![image](https://github.com/LuisVCSilva/hackaton/assets/23017780/9a9c3180-cb80-4ec2-8d76-0aa45ac62a62)---
datapackage:
  title: Dataset Template
  description: A template for a dataset to publish on DataHub. Uses the Data Package metadata.
  licenses:
  - path: http://opendatacommons.org/licenses/pddl/
    title: Open Data Commons Public Domain Dedication and License v1.0
  resources:
  - path: data.csv
    title: BTC - USD (2014 - 2024)
    name: btc-per-year
    format: csv
    schema:
      fields:
      - name: Date
        type: date
      - name: Open
        type: number
---


We can add a chart:

<LineChart
  data="./data.csv"
  title="BTC - USD (2014 - 2024) Open"
  xAxis="year"
  yAxis="value"
/>
