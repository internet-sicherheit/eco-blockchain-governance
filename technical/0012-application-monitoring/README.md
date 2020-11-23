# 0012: Application monitoring
- Authors: [David Maas](david_maas@hotmail.de) 
- Status: PROPOSED
- Since: 2020-10-21 
- Status Note: Initial Proposal  
- Start Date: 2020-10-21 
- Tags: 

## Summary
Specifies the monitoring of the applications

## Motivation

Due to the decentralised infrastructure, the monitoring of the applications is particularly important. In order to prevent misuse and manipulation, the monitoring of the applications is essential. However, the decentralised architecture makes this even more complex to implement.  

## Specification

The following points should be included in the application monitoring:
* Selection of the components to be monitored
* Definition of sampling rates
* Selection of the measuring method in the network
* Selection of applications
* Selection of the detection method
* Display of the measured values
* Selection of the analysis method
* Selection of the visualisation technology
* Selection of the alarm method
* Carrying out appropriate analyses
* Evaluation of event logs


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

The decentralised architecture makes logging much more complex
The decentralised architecture makes application monitoring much more complex 


## Prior art

Further information can be found at [Hyperledger Besu Monitor Metrics](https://besu.hyperledger.org/en/stable/HowTo/Monitor/Metrics/)

## Unresolved questions

* Standard application parameters must be defined to unify the monitoring of applications and make them compatible with any Blockchain network. 