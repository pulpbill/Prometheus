# Prometheus
Prometheus/Grafana from Helm charts to monitor K8s cluster

### Note:
This guide asumes that you have a running K8s cluster and helm installed (We'll be using helm's charts)
* I recommend instances type similar to t2.medium or bigger

## First steps:

### Installing Grafana:

Install from latest stable Helm chart:
```
helm install stable/grafana --name grafana-testing
```
I choose the helm release name "grafana-testing"
#### Pay attention, or better, copy the final lines from the output starting at "Notes: " You will need it.


### Installing Prometheus:
Install from latest stable Helm chart:
```
helm install stable/prometheus --name prometheus-testing
```
I choose the helm release name "prometheus-testing"
#### Pay attention, or better, copy the final lines from the output starting at "Notes: " You will need it.

Check your helm releases:
```
helm ls
```
