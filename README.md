This is a test to see if we can use Mermaid to create a graph representing iTop verions.

Useful links :
- Mermaid reference : https://mermaid-js.github.io/mermaid/#/
- GitHub support : https://github.blog/2022-02-14-include-diagrams-markdown-files-mermaid/


```mermaid
%%{init: { 'logLevel': 'debug', 'theme': 'base', 'gitGraph': {'mainBranchName': 'develop'}} }%%
gitGraph
    commit id: "2020-05-06" type: HIGHLIGHT tag: "v2.7.0-2"
    branch support/2.7
    commit id: "2020-06-26" tag: "2.7.1"
    commit id: "2020-11-10" tag: "2.7.2-1"
    commit id: "2020-12-09" tag: "2.7.3"
    commit id: "2021-03-31" tag: "2.7.4"
    commit id: "2021-04-06" tag: "3.0.0-beta"
    commit id: "2021-05-17" tag: "2.7.3-2"
    commit id: "2021-07-05" tag: "2.7.5"
    checkout develop
    commit id: "2021-07-05" type: REVERSE tag: "3.0.0-beta2"
    checkout support/2.7
    commit id: "2021-07-20" tag: "2.7.5-1"
    commit id: "2021-12-17" tag: "2.7.6"
    checkout develop
    commit id: "2022-01-04" type: HIGHLIGHT tag: "v3.0.0"
    commit id: "2022-01-04" tag: "3.0.0"
    commit id: "2022-04-08" tag: "3.0.1"
```

Nice Excel formula to get the commit text :
```excel
=CONCATENER("commit id: """;TEXT(A52,"yyyy-mm-dd");""" tag: """;C52;"""");
```