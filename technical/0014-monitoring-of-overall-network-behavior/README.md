# 0014: Monitoring of overall network behavior
- Authors: [David Maas](david_maas@hotmail.de) 
- Status: PROPOSED
- Since: 2020-10-21 
- Status Note: Initial Proposal  
- Start Date: 2020-10-21 
- Tags: 

## Summary
Describes the monitoring of the entire network behaviour.

## Motivation
To detect problems and security risks at an early stage, monitoring of the entire Blockchain network is necessary. Due to the decentralised architecture, however, this monitoring is considerably more complex. 

## Specification
The following criteria should be considered when monitoring the overall network behaviour: 

* Selection of monitoring areas
* Selection of the measured variables
* Selection of sensor technology
* Definition of sampling rates
* Selection of the transmission protocols
* Operation of a separate surveillance network
* Monitoring in SAN
* Network performance monitoring
* Selection of the measuring method in the network
* Use of TAPs
* Monitoring the quality of service
* Monitoring network software / services
* Monitoring of the network components
* Selection of the detection method
* Display of the measured values
* Selection of the analysis method
* Selection of the visualisation technology
* Selection of the alarm method
* Use of early detection 
* Collection of historical data
* Evaluation of event logs
* Event Correlation
* Trend analysis



## Examples & Best Practices
There are many monitoring tools for Blockchain Networks. The metrics and logs can be used to draw conclusions about the network. 

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
The decentralised architecture makes network monitoring much more complex 

## Prior art
Further information can be found at [Hyperledger Besu Monitor Metrics](https://besu.hyperledger.org/en/stable/HowTo/Monitor/Metrics/)


## Unresolved questions
A collection of all network data of all nodes is quite complex and would have to be timed correctly. The resulting data must be processed sensibly for an automated analysis and the resulting conclusions and reactions. AI-based procedures would be suitable for this. 