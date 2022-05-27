This is a test to see if we can use Mermaid to create a graph representing iTop verions.

Useful links :
- Mermaid reference : https://mermaid-js.github.io/mermaid/#/
- GitHub support : https://github.blog/2022-02-14-include-diagrams-markdown-files-mermaid/


```mermaid
%%{init: { 'logLevel': 'debug', 'theme': 'base', 'gitGraph': {'showBranches': true,'mainBranchName': 'develop'}} }%%
gitGraph
    commit id: "2016-07-06" tag: "2.3.0"
    branch support/2.3
    commit id: "2016-07-08" tag: "2.3.1"
    commit id: "2016-12-22" tag: "2.3.3"
    commit id: "2017-04-14" tag: "2.3.4"
    checkout develop
    commit id: "2017-07-12" tag: "2.4.0-beta" type: REVERSE
    commit id: "2017-11-15" tag: "2.4.0"
    commit id: "2017-11-16" tag: "2.4.0"
    branch support/2.4
    commit id: "2018-02-14" tag: "2.4.1"
    checkout develop
    commit id: "2018-04-25" tag: "2.5.0-beta" type: REVERSE
    checkout support/2.4
    commit id: "2018-06-14" tag: "2.4.2"
    checkout develop
    commit id: "2018-06-27" tag: "2.5.0"
    branch support/2.5
    commit id: "2019-01-09" tag: "2.6.0"
    branch support/2.6
    commit id: "2019-03-28" tag: "2.6.1"
    commit id: "2019-07-24" tag: "2.6.2-1"
    branch support/2.6.2
    commit id: "2019-10-07" tag: "2.6.2-2"
    checkout develop
    commit id: "2019-12-18" tag: "2.7.0-beta" type: REVERSE
    checkout support/2.5
    commit id: "2020-01-22" tag: "2.5.4"
    checkout support/2.6
    commit id: "2020-01-23" tag: "2.6.3"
    checkout develop
    commit id: "2020-01-29" tag: "2.7.0-beta2" type: REVERSE
    commit id: "2020-04-01" tag: "2.7.0-1"
    branch support/2.7
    checkout support/2.6
    commit id: "2020-04-22" tag: "2.6.4"
    checkout develop
    commit
    branch support/2.7.0
    commit id: "2020-05-06" tag: "2.7.0-2"
    checkout support/2.7
    commit id: "2020-06-26" tag: "2.7.1"
    commit id: "2020-11-10" tag: "2.7.2-1"
    commit id: "2020-12-09" tag: "2.7.3"
    branch support/2.7.3
    checkout support/2.7
    commit id: "2021-03-31" tag: "2.7.4"
    checkout develop
    commit id: "2021-04-06" tag: "3.0.0-beta" type: REVERSE
    checkout support/2.7.3
    commit id: "2021-05-17" tag: "2.7.3-2"
    checkout support/2.7
    commit id: "2021-07-05" tag: "2.7.5"
    branch support/2.7.5
    checkout develop
    commit id: "2021-07-05." tag: "3.0.0-beta2" type: REVERSE
    checkout support/2.7.5
    commit id: "2021-07-20" tag: "2.7.5-1"
    checkout support/2.7
    commit id: "2021-12-17" tag: "2.7.6"
    checkout develop
    commit id: "2022-01-04" tag: "3.0.0"
    branch support/3.0
    commit id: "2022-04-08" tag: "3.0.1"
```

Nice Excel formula to get the commit text :
```excel
=CONCATENER("commit id: """;TEXT(A52,"yyyy-mm-dd");""" tag: """;C52;"""");
```