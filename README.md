#  Dynatrace-Kafka-Plugin
The Dynatrace-Kafka-Plugin is based on the JMX Plugin and allows the Dynatrace OneAgent to collect JMX based metrics associated with the Kafka Broker, Kafka Consumers and Kafka Producers. 

## Requirements
* Dynatrace Environment with OneAgent Installed on Kafka hosts
* Dynatrace Environment permissions to upload custom plugins
## Installation
OneAgent Plugins need to get installed both, on you Tenant and on the host(s) they are supposed to collect data for - mainly for security reasons. NO third party code is getting executed by your OneAgent unless your Tenant and your Agent agree on the authenticity of your plugin.
This is why you need to install, in addition to your Tenant, on selected Hosts, that have OneAgent running and are supposed to execute your Plugin.
## Installation on your Dynatrace Tenant
* From the 'Settings' -> 'Monitoring' -> 'Monitored Technologies' section, select 'Custom plugins' tab
* Click on the button 'Upload Plugin' and select the Kafka.json files you wish to use.

## Limitations
* JMX monitoring is highly dynamic. If a particular metric doesn’t exist in your JVM, it's not an error—the metric simply isn't available.

## Important links:

https://www.dynatrace.com/support/help/monitoring-plugins/application-plugins/how-do-i-monitor-jmx-metrics-in-my-java-applications/ 

 https://dynatrace.github.io/plugin-sdk/api/plugin_json_apidoc.html
