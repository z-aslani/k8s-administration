# Kubernetes Administration

## Summary:
This repository includes all resources including automations, configuration-as-codes, etc. for administrating Pegah Kubernetes Clusters.

## Administration Parts:

### Kubernetes Upgrade

#### Ansible
whole-cluster upgrade procedures written as `Ansible` playbooks supporting HA and non-HA control planes.

Playbook Arguments:
* k8s_cluster: `("production"|"staging")`
* upgrade_cni: `(true|false)`
* network_plugin: `(weavenet|calico)`
* k8s_cluster_pod_cidr: e.g. `192.168.0.0/16`
* allow_prerequisites: `(true|false)`


__Warning__: This playbook has not been thoroughly tested yet and is a work in progress.
