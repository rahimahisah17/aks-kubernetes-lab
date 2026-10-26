# AKS FinOps Cost Report

## Cluster Configuration
- Resource Group: rg-aks-lab
- Cluster: aks-lab
- Region: westeurope
- Node Pool: nodepool1
- VM Size: Standard_D2s_v3
- Node Count: 1

## Resource Utilization
- Node CPU usage: 12%
- Node memory usage: 25%
- CPU requests: 62%
- Memory requests: 22%

## Cost Estimate
- Estimated VM rate: $0.12/hour
- Estimated monthly VM cost (730 hours): $87.60
- Estimate excludes additional AKS and Azure resource charges.

## Cost Optimization Actions
- Configured web deployment autoscaling between 1 and 5 replicas.
- Enabled cluster autoscaling for nodepool1 between 1 and 3 nodes.
- Reduced the node pool to 1 node.
- Removed the web-public LoadBalancer service.
- Stopped the AKS cluster when not in use.

## Notes
The VM price is a public retail-price estimate, not a confirmed invoice amount. Actual costs depend on billing rates and associated Azure resources.
