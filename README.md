# Containerisation of React and MongoDB

### The Swimlane project is Dockerised and the image is published to dockerhub with the name : 

```
kellydockerhub/swimlane-react
```
We would be using this docker image to deploy our code into the kubernetes cluster 

### Next  steps - Using Terraform to EKS Cluster

Terraform scripts would create the whole EKS cluster and the associated infra related to it in AWS. A new cluster will be created in us-east-2 AWS region by default


### You can use helm to deploy the chart into the cluster

Pre-requisites : Helm 3 should be installed 

1) Navigate to helm/swimlane
```
helm install swimlane swimlane 
```
2) Uninstalling a chart
```
helm uninstall swimlane 
```
