# insecure-k8s
 Example of an insecure Kubernetes cluster
This EKS cluster has been puposefully misconfigured to display how miconfigurations in a K8s can be exploited by the attackers.

![alt text] (https://github.com/vdhar71/insecure-k8s/blob/main/insecure-k8s.png)

Start with creating an EKS Kubernetes:
```
eksctl create cluster -f cluster.yaml
```
NOTE: DO NOT TRY TO CREATE AN EKS CLUSTER IN AN EXISTING VPC. EKS Cloud Formation stackset requires/creates various AWS resources that is impossible to create them in an existing VPC.  Refer: (https://eksctl.io/usage/creating-and-managing-clusters/)
