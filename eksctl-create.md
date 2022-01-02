```
eksctl create cluster --name=scala-hello-world --nodes=1 --node-type t3a.nano --region us-east-2
2022-01-01 22:21:49 [ℹ]  eksctl version 0.77.0
2022-01-01 22:21:49 [ℹ]  using region us-east-2
2022-01-01 22:21:50 [ℹ]  setting availability zones to [us-east-2c us-east-2b us-east-2a]
2022-01-01 22:21:50 [ℹ]  subnets for us-east-2c - public:192.168.0.0/19 private:192.168.96.0/19
2022-01-01 22:21:50 [ℹ]  subnets for us-east-2b - public:192.168.32.0/19 private:192.168.128.0/19
2022-01-01 22:21:50 [ℹ]  subnets for us-east-2a - public:192.168.64.0/19 private:192.168.160.0/19
2022-01-01 22:21:50 [ℹ]  nodegroup "ng-7f7fb508" will use "" [AmazonLinux2/1.21]
2022-01-01 22:21:50 [ℹ]  using Kubernetes version 1.21
2022-01-01 22:21:50 [ℹ]  creating EKS cluster "scala-hello-world" in "us-east-2" region with managed nodes
2022-01-01 22:21:50 [ℹ]  will create 2 separate CloudFormation stacks for cluster itself and the initial managed nodegroup
2022-01-01 22:21:50 [ℹ]  if you encounter any issues, check CloudFormation console or try 'eksctl utils describe-stacks --region=us-east-2 --cluster=scala-hello-world'
2022-01-01 22:21:50 [ℹ]  CloudWatch logging will not be enabled for cluster "scala-hello-world" in "us-east-2"
2022-01-01 22:21:50 [ℹ]  you can enable it with 'eksctl utils update-cluster-logging --enable-types={SPECIFY-YOUR-LOG-TYPES-HERE (e.g. all)} --region=us-east-2 --cluster=scala-hello-world'
2022-01-01 22:21:50 [ℹ]  Kubernetes API endpoint access will use default of {publicAccess=true, privateAccess=false} for cluster "scala-hello-world" in "us-east-2"
2022-01-01 22:21:50 [ℹ]  
2 sequential tasks: { create cluster control plane "scala-hello-world", 
    2 sequential sub-tasks: { 
        wait for control plane to become ready,
        create managed nodegroup "ng-7f7fb508",
    } 
}
2022-01-01 22:21:50 [ℹ]  building cluster stack "eksctl-scala-hello-world-cluster"
2022-01-01 22:21:50 [ℹ]  deploying stack "eksctl-scala-hello-world-cluster"
2022-01-01 22:22:20 [ℹ]  waiting for CloudFormation stack "eksctl-scala-hello-world-cluster"
2022-01-01 22:22:51 [ℹ]  waiting for CloudFormation stack "eksctl-scala-hello-world-cluster"
2022-01-01 22:23:51 [ℹ]  waiting for CloudFormation stack "eksctl-scala-hello-world-cluster"
2022-01-01 22:24:51 [ℹ]  waiting for CloudFormation stack "eksctl-scala-hello-world-cluster"
2022-01-01 22:25:52 [ℹ]  waiting for CloudFormation stack "eksctl-scala-hello-world-cluster"
2022-01-01 22:26:52 [ℹ]  waiting for CloudFormation stack "eksctl-scala-hello-world-cluster"
2022-01-01 22:27:52 [ℹ]  waiting for CloudFormation stack "eksctl-scala-hello-world-cluster"
2022-01-01 22:28:53 [ℹ]  waiting for CloudFormation stack "eksctl-scala-hello-world-cluster"
2022-01-01 22:29:53 [ℹ]  waiting for CloudFormation stack "eksctl-scala-hello-world-cluster"
2022-01-01 22:30:53 [ℹ]  waiting for CloudFormation stack "eksctl-scala-hello-world-cluster"
2022-01-01 22:31:53 [ℹ]  waiting for CloudFormation stack "eksctl-scala-hello-world-cluster"
2022-01-01 22:32:54 [ℹ]  waiting for CloudFormation stack "eksctl-scala-hello-world-cluster"
2022-01-01 22:33:54 [ℹ]  waiting for CloudFormation stack "eksctl-scala-hello-world-cluster"
2022-01-01 22:34:54 [ℹ]  waiting for CloudFormation stack "eksctl-scala-hello-world-cluster"
2022-01-01 22:36:57 [ℹ]  building managed nodegroup stack "eksctl-scala-hello-world-nodegroup-ng-7f7fb508"
2022-01-01 22:36:58 [ℹ]  deploying stack "eksctl-scala-hello-world-nodegroup-ng-7f7fb508"
2022-01-01 22:36:58 [ℹ]  waiting for CloudFormation stack "eksctl-scala-hello-world-nodegroup-ng-7f7fb508"
2022-01-01 22:37:14 [ℹ]  waiting for CloudFormation stack "eksctl-scala-hello-world-nodegroup-ng-7f7fb508"
2022-01-01 22:37:32 [ℹ]  waiting for CloudFormation stack "eksctl-scala-hello-world-nodegroup-ng-7f7fb508"
2022-01-01 22:37:51 [ℹ]  waiting for CloudFormation stack "eksctl-scala-hello-world-nodegroup-ng-7f7fb508"
2022-01-01 22:38:08 [ℹ]  waiting for CloudFormation stack "eksctl-scala-hello-world-nodegroup-ng-7f7fb508"
2022-01-01 22:38:29 [ℹ]  waiting for CloudFormation stack "eksctl-scala-hello-world-nodegroup-ng-7f7fb508"
2022-01-01 22:38:48 [ℹ]  waiting for CloudFormation stack "eksctl-scala-hello-world-nodegroup-ng-7f7fb508"
2022-01-01 22:39:07 [ℹ]  waiting for CloudFormation stack "eksctl-scala-hello-world-nodegroup-ng-7f7fb508"
2022-01-01 22:39:24 [ℹ]  waiting for CloudFormation stack "eksctl-scala-hello-world-nodegroup-ng-7f7fb508"
2022-01-01 22:39:42 [ℹ]  waiting for CloudFormation stack "eksctl-scala-hello-world-nodegroup-ng-7f7fb508"
2022-01-01 22:39:59 [ℹ]  waiting for CloudFormation stack "eksctl-scala-hello-world-nodegroup-ng-7f7fb508"
2022-01-01 22:40:00 [ℹ]  waiting for the control plane availability...
2022-01-01 22:40:00 [✔]  saved kubeconfig as "/Users/kevinmeredith/.kube/config"
2022-01-01 22:40:00 [ℹ]  no tasks
2022-01-01 22:40:00 [✔]  all EKS cluster resources for "scala-hello-world" have been created
2022-01-01 22:40:00 [ℹ]  nodegroup "ng-7f7fb508" has 1 node(s)
2022-01-01 22:40:00 [ℹ]  node "ip-192-168-92-44.us-east-2.compute.internal" is ready
2022-01-01 22:40:00 [ℹ]  waiting for at least 1 node(s) to become ready in "ng-7f7fb508"
2022-01-01 22:40:00 [ℹ]  nodegroup "ng-7f7fb508" has 1 node(s)
2022-01-01 22:40:00 [ℹ]  node "ip-192-168-92-44.us-east-2.compute.internal" is ready
2022-01-01 22:40:02 [ℹ]  kubectl command should work with "/Users/kevinmeredith/.kube/config", try 'kubectl get nodes'
2022-01-01 22:40:02 [✔]  EKS cluster "scala-hello-world" in "us-east-2" region is ready
$
```