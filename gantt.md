
* Gantt reference : https://mermaid-js.github.io/mermaid/#/./gantt
* ➕ Benefits
  - vertical bars, easier to see versions per year
* ➖ Drawbacks
  - task duration is mandatory, cannot say "until child start"
  - hard to see hierarchy/graph



```mermaid
gantt
  title iTop versions history
  dateFormat  YYYY-MM-DD
  section 2.7
  2.7.0      :2.7.0, 2020-01-29, 2020-06-26
  2.7.1      :after 2.7.0, 2020-06-26, 2020-12-09
  2.7.3      :after 2.7.1, 2020-12-09, 1w
```