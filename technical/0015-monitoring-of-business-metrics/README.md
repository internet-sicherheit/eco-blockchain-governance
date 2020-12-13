# 0015: Monitoring of business metrics
- Authors: [David Maas](david_maas@hotmail.de) 
- Status: PROPOSED
- Since: 2020-10-21 
- Status Note: Initial Proposal  
- Start Date: 2020-10-21 
- Tags: 

## Summary
Describes the monitoring of business metrics

## Motivation
By monitoring business metrics, one can draw conclusions about the blockchain network in general, but also make optimisations to optimise revenues and reduce expenses. Therefore, it is highly recommended to use the business metrics.

## Specification

The following metrics are measurable in a blockchain network: 
* Active Nodes (Active Addresses)
* Active Nodes
* Blocks Per Hour, Blocks Per Day
* Transactions Per Second
* Transaction Latency
* Transaction Throughput
* Full Node/Partial Node Ratio

From this, it should be possible to draw conclusions about the following points:
* reducing transaction costs
* increasing revenues due to increased amount of transactions
* creating new revenue streams due to lowered transaction costs
* reducing level of required capital
* increasing capital usage or employability

These represent parameters for the business metrics that should be identified.

## Examples & Best Practices
There are many monitoring tools for Blockchain Networks. The metrics and logs can be used to draw conclusions about the applications. 

[Hyperledger Besu](https://besu.hyperledger.org/en/stable/HowTo/Monitor/Metrics/) uses the following tools: 

>Use metrics to monitor node performance
To enable the Prometheus monitoring and alerting service to access Hyperledger Besu metrics, use the --metrics-enabled option. Use Grafana to visualize the collected data. See the sample Besu Grafana dashboard.

[Features of Prometeus:](https://prometheus.io/docs/introduction/overview/)
>Prometheus's main features are:

>* a multi-dimensional data model with time series data identified by metric name and key/value pairs
>* PromQL, a flexible query language to leverage this dimensionality
>* no reliance on distributed storage; single server nodes are autonomous
>* time series collection happens via a pull model over HTTP
>* pushing time series is supported via an intermediary gateway
>* targets are discovered via service discovery or static configuration
>* multiple modes of graphing and dashboarding support

[Features of Grafana:](https://grafana.com/grafana/)

>Built-in Prometheus Support
* Query editor with metric name lookup
* Templating queries for generic dashboards
* Alias patterns for short readable series names

## Drawbacks
By focusing on optimisations through business metrics, opposite effects can occur. Among them, for example, congestion due to lowered transaction costs.

## Prior art
Further information can be found at [Hyperledger Besu Monitor Metrics](https://besu.hyperledger.org/en/stable/HowTo/Monitor/Metrics/)

## Unresolved questions
Of particular interest in this context is the monitoring of the entire network and the information gained from the business metrics for automatic optimisation. AI analysis and further processing of the data result in fully automated processes that still need to be developed.