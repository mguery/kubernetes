# kubernetes

## Basics



**Resources**

[Cloud-Native repo - Docker & K8s notes](https://github.com/mguery/cloud-native#lesson-3-container-orchestration-with-kubernetes)
[DevOps Notes - Kubernetes](https://github.com/bregman-arie/devops-exercises#kubernetes)

---

## Kubernetes: Monitoring with Prometheus

[Notes from LinkedIn course](https://www.linkedin.com/learning/kubernetes-monitoring-with-prometheus/logging-vs-monitoring)

> In order to prevent outages, it's essential that you leverage a monitoring and alerting tool in your Kubernetes environment. Prometheus—an open-source systems monitoring and alerting toolkit—pairs particularly well with Kubernetes. In this course, learn how this toolkit integrates with Kubernetes and works to monitor distributed systems.

**Logging vs. monitoring**
logs are qualitative =, time series-based and metrics are point-in-time data points that have some meta data around them.

**Monitoring K8s**
There's cAdvisor, Heapster, and Prometheus. Prometheus is a pull-based time-series capture, storage, and alerting service with Kubernetes integration.

**Enabling Prometheus monitoring**
from promoperator.yml file - creating accounts, roles, binding. `kube control create -f`
[verbs: "\*"] = * all verbs (can create, read, watch, update, delete)

create service endpoints - exposes tools like Prom to other apps

