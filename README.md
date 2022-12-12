# Containerisation of React and MongoDB

### Using Helm 

Pre-requisites : Helm 3 should be installed 

1) Navigate to helm/swimlane
```
helm install swimlane swimlane 
```
2) Uninstalling a chart
```
helm uninstall swimlane 
```

### Using Terraform

Terraform scripts would create the whole EKS cluster and the associated infra related to it in AWS. A new cluster will be created in us-east-2 AWS region by default
