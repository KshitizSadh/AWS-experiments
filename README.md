# AWS-experiments
## What is cloud computing
- cloud computing is the delivery of computing services including servers,storage,databases,networking,software etc.
## benfits 
- faster time to market
- scalability and flexibility
- cost savings
- better collaboration
- advanced security
- data loss prevention
## disadvantage 
- risk of vendor lock-in
- less control over underlying cloud insfra
- concerns about security risks like data privacy and online threats
- integration complexity with exisiting systems
- unforseen costs and unexpected expenses

![pic1](https://github.com/KshitizSadh/AWS-experiments/assets/142923024/fc5557a2-57f2-48b6-b393-bc3358c22b1e)

- example of private implementation softwares : openstack , opennebula 


## Hyperscalars : A hyperscaler is a type of large-scale data center that offers massive computing resources, typically in the form of an elastic cloud platform. Organizations use them to deploy and manage large-scale applications and services.

![1](https://github.com/KshitizSadh/AWS-experiments/assets/142923024/21edfca6-ace3-40d4-85c5-763834a984cd)
![2](https://github.com/KshitizSadh/AWS-experiments/assets/142923024/b8df980e-01d3-47f8-aa93-09de6ba5c949)


## Compute services 
- EC2  
- ECS/EKS : containerized services `
  - Fargate
- lambda : serverless 

## Storage Services
- S3
- EBS : Amazon Elastic Block Storage is a storage service wherein each block of storage acts like a separate hard drive (volume) . 
- EFS : dont need to assign any volume , can do on its own , seamless storage , database on EC2 instances 
- Archival service - Glacier : Amazon Glacier is extremely low cost, secure, and durable storage service for data archiving and
backup. That data stored which are not needed instantly , eg old data . Takes time min 4 hours or 1 day to retrieve request ( S3 instantly returns request)

## Network Services
- VPC : own insolated environment in a public cloud
- Domain Name Service - Route 53

![3](https://github.com/KshitizSadh/AWS-experiments/assets/142923024/d935eda9-c3c1-42b7-ad83-f155663f230a)

- public subnet : can receive traffic from outerworld 
- private subnet : cannot receive traffic from outerworld but may or may not send traffic to outerworld

![4](https://github.com/KshitizSadh/AWS-experiments/assets/142923024/685a89b5-624e-4317-865a-ffd028b86e0a)

![5](https://github.com/KshitizSadh/AWS-experiments/assets/142923024/c1eac689-affe-4ee1-9ab9-c12c9ccee161)

![6](https://github.com/KshitizSadh/AWS-experiments/assets/142923024/c24c2de0-75ca-4449-885a-8fd207acfa18)

![7](https://github.com/KshitizSadh/AWS-experiments/assets/142923024/c4be8b85-ff5f-4d75-9079-4902cf7315f1)

![8](https://github.com/KshitizSadh/AWS-experiments/assets/142923024/60f36d04-b892-43b6-8784-b1c8aec39bdd)

![9](https://github.com/KshitizSadh/AWS-experiments/assets/142923024/4c6e22f0-1a9c-4473-8064-4784a9ef4416)

![10](https://github.com/KshitizSadh/AWS-experiments/assets/142923024/2f10ab4b-bbfd-4ada-add5-658538244d19)

- **Apache web server works on layer 7 , using single apache server one can deploy multiple applications on different ports based on paths (URLbased) (virtual hosts) . virtual hosting can only work on layer 7**

## Application based LB 
- key pair : kind of like a password (public key is username; private key is password)
  - PPK (PuTTY Private Key) and PEM (Privacy Enhanced Mail) are two file formats that are commonly used for SSH and SSL/TLS connections. While PPK files are primarily used with PuTTY on Windows, PEM files are more widely supported and can be used with various tools and platforms

- security groups : A security group controls the traffic that is allowed to reach and leave the resources that it is associated with. For example, after you associate a security group with an EC2 instance, it controls the inbound and outbound traffic for the instance. When you create a VPC, it comes with a default security group. (acts as a firewall)

![11](https://github.com/KshitizSadh/AWS-experiments/assets/142923024/f2799c43-c532-4566-a9df-6571e2007462)

![12](https://github.com/KshitizSadh/AWS-experiments/assets/142923024/498ab7fc-edb7-4895-ab79-0bbbc02c3a7f)

![13](https://github.com/KshitizSadh/AWS-experiments/assets/142923024/470981f0-3fe6-4f64-b68f-e8fc88f5f6e0)

![15](https://github.com/KshitizSadh/AWS-experiments/assets/142923024/41772bc6-0463-40fe-b14b-57750d25c9fd)


### Creating a target group  

- Your load balancer routes requests to the targets in a target group and performs health checks on the targets.
- LB routes traffic to target group then traffic group routes traffic to the back end ec2 instances or IP addresses etc
  
![16](https://github.com/KshitizSadh/AWS-experiments/assets/142923024/5854f26e-8508-4736-b304-6a025ca40e31)
![17](https://github.com/KshitizSadh/AWS-experiments/assets/142923024/f1ec0251-58b8-45c6-9185-14f41a8897c0)
![18](https://github.com/KshitizSadh/AWS-experiments/assets/142923024/b9e39e05-8584-4756-ba13-eac93fc9e2ea)
![19](https://github.com/KshitizSadh/AWS-experiments/assets/142923024/650e9e64-b0ab-483a-b20a-0e19cd97585e)

## Autoscalling 
![20](https://github.com/KshitizSadh/AWS-experiments/assets/142923024/a48f6352-8d63-432b-bcaf-beb28b07737b)

### Creating launch template
![21](https://github.com/KshitizSadh/AWS-experiments/assets/142923024/f7e315d0-260f-4a9c-82ae-452b2ee22e1d)
![22](https://github.com/KshitizSadh/AWS-experiments/assets/142923024/01dfcd37-999c-475c-a4df-3a43c70b88b0)
![23](https://github.com/KshitizSadh/AWS-experiments/assets/142923024/e878a457-b14a-46e7-8321-f3bd95a371a1)
![24](https://github.com/KshitizSadh/AWS-experiments/assets/142923024/055bd32a-ea77-43fd-928e-88b1e27ba7c3)
![25](https://github.com/KshitizSadh/AWS-experiments/assets/142923024/e5131c56-7f52-4cbc-baf4-1daed3ceee78)
![26](https://github.com/KshitizSadh/AWS-experiments/assets/142923024/6fac9546-4693-4757-adc8-2012064a984b)
![27](https://github.com/KshitizSadh/AWS-experiments/assets/142923024/6dd37431-cfd3-4845-8c2a-b9fedba2f0c7)
![28](https://github.com/KshitizSadh/AWS-experiments/assets/142923024/561b0b44-f2da-444f-b19d-fadc5875b6e4)

### Creating scalling policies 
![29](https://github.com/KshitizSadh/AWS-experiments/assets/142923024/b371812f-0100-43cb-80d8-a4109c165fea)
![30](https://github.com/KshitizSadh/AWS-experiments/assets/142923024/7f0818b1-ec26-4463-8a2b-6a8ccb0c76ba)

## Artificial load 
``` bash
htop
```
![31](https://github.com/KshitizSadh/AWS-experiments/assets/142923024/4173f154-3fd0-44fb-9402-b75443abdcaf)

- currently 0

- making instance count to a high number
``` bash
seq 999999999999999999999 > /dev/null &
```

![32](https://github.com/KshitizSadh/AWS-experiments/assets/142923024/f0acb39f-f22e-455c-bf04-308c4bbe7717)
![33](https://github.com/KshitizSadh/AWS-experiments/assets/142923024/6102b032-4096-472a-99e6-57b7e4e72c9e)
![34](https://github.com/KshitizSadh/AWS-experiments/assets/142923024/6c6ec8e3-4b7d-436d-b7a6-0491bfb6f3bb)
![35](https://github.com/KshitizSadh/AWS-experiments/assets/142923024/c26e8c03-7711-4e88-9dce-356c411991dc)

- going to the DNS name and reloading will take you to diff targets(3)
- this is **round robin** at work  

## AWS CLI : The AWS Command Line Interface (AWS CLI) is a unified tool to manage your AWS services. With just one tool to download and configure, you can control multiple AWS services from the command line and automate them through scripts.
- BOTO library in python

![Screenshot from 2023-11-27 16-45-38](https://github.com/KRIISHSHARMA/AWS/assets/86760658/fae33c2d-6122-4ee2-aa75-5f061bcbba20)
![Screenshot from 2023-11-27 16-47-42](https://github.com/KRIISHSHARMA/AWS/assets/86760658/768d5a91-8c74-42ed-b08e-14c3ad5c11eb)

``` bash
sudo snap install aws-cli
```
``` bash
aws configure
```
![Screenshot from 2023-11-27 17-08-27](https://github.com/KRIISHSHARMA/AWS/assets/86760658/71a8036d-299a-4b48-adbb-8049b3f16dea)

- in security credentials , before creating access key copy and paste PU , PrK and fill location and format in terminal 
- give user access

![Screenshot from 2023-11-27 17-30-18](https://github.com/KRIISHSHARMA/AWS/assets/86760658/50c16ed9-0a30-49a2-b9aa-d834c2622e99)


- after creating instance
``` bash
aws ec2 describe-instances
``` 

![Screenshot from 2023-11-27 17-35-01](https://github.com/KRIISHSHARMA/AWS/assets/86760658/e4ba62f0-42f5-4e8d-840f-41d32e1cf6a3)
![Screenshot from 2023-11-27 17-35-01](https://github.com/KRIISHSHARMA/AWS/assets/86760658/de7fef08-39e8-4525-a276-6da3f8c2e742)
![Screenshot from 2023-11-27 17-46-10](https://github.com/KRIISHSHARMA/AWS/assets/86760658/15f77e24-064b-4aca-9de0-562c6a54c890)
![Screenshot from 2023-11-27 18-12-04](https://github.com/KRIISHSHARMA/AWS/assets/86760658/1cf4f02a-59c8-43d9-896f-28d980add612)
![Screenshot from 2023-11-27 18-12-32](https://github.com/KRIISHSHARMA/AWS/assets/86760658/6e9a8d71-0ede-42fd-9c93-3a53a2e109a0)
![Screenshot from 2023-11-27 18-14-02](https://github.com/KRIISHSHARMA/AWS/assets/86760658/899d441d-7208-4778-8537-6be1a92008d0)
![Screenshot from 2023-11-27 18-17-35](https://github.com/KRIISHSHARMA/AWS/assets/86760658/89a6f2f4-a014-4ec6-91fe-4994d0e26d40)
![Screenshot from 2023-11-27 18-26-06](https://github.com/KRIISHSHARMA/AWS/assets/86760658/4789776e-d9e7-4a27-8c3d-038298c02daf)


- docker image to create art load
- pods : Pods are the smallest deployable units of computing that you can create and manage in Kubernetes. A Pod (as in a pod of whales or pea pod) is a group of one or more containers, with shared storage and network resources, and a specification for how to run the containers.

 ![download](https://github.com/KRIISHSHARMA/AWS/assets/86760658/1bf8d1eb-e0b6-4674-bd98-fbcf383135d3)

- daemon sets : works on nodes where pods are running , can manage all your agents eg if we are runninf 5 ec2 instances behind the k8s cluster then we can run 1 daemon set and that daemon set wil take care of all the agents 

## CLOUD 9
- cloud based IDE (vscode , pycharm etc)
- provides IDE on browsers

![Screenshot from 2023-12-02 16-01-33](https://github.com/KRIISHSHARMA/AWS/assets/86760658/9208cded-f435-451a-a192-c4a254244e75)
![Screenshot from 2023-12-02 16-12-26](https://github.com/KRIISHSHARMA/AWS/assets/86760658/9efd1bc2-5393-4ac1-9a28-0355a7961482)
![Screenshot from 2023-12-02 16-12-51](https://github.com/KRIISHSHARMA/AWS/assets/86760658/b7a5eecb-5d92-46af-a9ad-7ba6db2a5391)


- after confiugring aws cli on cloud 9 (scroll up) 
-  configure EKS ctl and kubectl [link for installation](https://docs.aws.amazon.com/emr/latest/EMR-on-EKS-DevelopmentGuide/setting-up-eksctl.html)
  
![Screenshot from 2023-12-02 16-35-44](https://github.com/KRIISHSHARMA/AWS/assets/86760658/e128f431-c888-4cc3-b8fa-2f7a0a3835a1)
![Screenshot from 2023-12-02 16-55-57](https://github.com/KRIISHSHARMA/AWS/assets/86760658/79d1bb3c-b8b3-49af-bd3f-b7552ab700da)
![Screenshot from 2023-12-02 16-56-13](https://github.com/KRIISHSHARMA/AWS/assets/86760658/9e89cf9d-7dbc-419e-8f0b-f35c8b830198)
![Screenshot from 2023-12-02 16-57-22](https://github.com/KRIISHSHARMA/AWS/assets/86760658/7bd6650b-e499-414d-baef-5f7a5bdc8799)

- launching a cluster
  ```bash
  eksctl create cluster --name test --version 1.28 --nodegroup-name ng.default --node-type t3.micro --nodes 2 --managed
  ```
  ![Screenshot from 2023-12-02 17-05-19](https://github.com/KRIISHSHARMA/AWS/assets/86760658/460b3b95-798a-439f-9611-95c419fa1064)

- yaml file for nginx container launched with official nginx image
  ``` bash
     apiVersion: apps/v1
  kind: Deployment
  metadata:
      labels:
          environment: test
      name: test
  spec:
      replicas: 1
      selector:
          matchLabels:
               environment: test
      template:
          metadata:
              labels:
                  environment: test
          spec:
              containers:
              - image: nginx:1.16
                name: nginx

  ```
``` bash
  nano nginx-deployment.yaml
```
- kubectl is the thing using which we will be creating , launching the resources , creating pods , troubleshooting cluster using kubectl
- we will apply this file using kubectl
  ``` bash
    kubectl apply -f nginx-deployment.yaml
  ```
![Screenshot from 2023-12-02 17-51-03](https://github.com/KRIISHSHARMA/AWS/assets/86760658/1d1e3352-8c71-4714-91f4-b94a25168230)

- to see pods used by kubectl
![Screenshot from 2023-12-02 17-58-35](https://github.com/KRIISHSHARMA/AWS/assets/86760658/4621853e-23ea-4d95-be42-986136776895)

- autoscaler used by eks
![Screenshot from 2023-12-02 18-00-51](https://github.com/KRIISHSHARMA/AWS/assets/86760658/e926f3b6-ec65-43a1-854d-6c809c6680f4)

- can scale it 
![Screenshot from 2023-12-02 18-03-17](https://github.com/KRIISHSHARMA/AWS/assets/86760658/533bd710-6456-47ed-8235-266d641d31a9)

- install matrix server , will continue to moniter the cpu matrix ,without this will not show how much resources are utilised 
``` bash
kubectl apply -f https://github.com/kubernetes-sigs/metrics-server/releases/latest/download/components.yaml
```

- creating php-apache autoscaling yaml file for horizontal pod autoscaling
  ``` bash
  apiVersion: apps/v1
  kind: Deployment
  metadata:
    name: php-apache
  spec:
    selector:
      matchLabels:
        run: php-apache
    template:
      metadata:
        labels:
          run: php-apache
      spec:
        containers:
        - name: php-apache
          image: registry.k8s.io/hpa-example
          ports:
          - containerPort: 80
          resources:
            limits:
              cpu: 500m
            requests:
              cpu: 200m
  ---
  apiVersion: v1
  kind: Service
  metadata:
    name: php-apache
    labels:
      run: php-apache
  spec:
    ports:
    - port: 80
    selector:
      run: php-apache
  ---
  
  apiVersion: autoscaling/v1
  kind: HorizontalPodAutoscaler
  metadata:
    name: php-apache
    namespace: default
  spec:
    scaleTargetRef:
       apiVersion: apps/v1
       kind: Deployment
       name: php-apache
    minReplicas: 1
    maxReplicas: 10
    targetCPUUtilizationPercentage: 50
  ```

```  bash
nano hpa.yaml
```
- deploying
  ``` bash
  kubectl apply -f hpa.yaml
  ```
![Screenshot from 2023-12-02 18-46-22](https://github.com/KRIISHSHARMA/AWS/assets/86760658/95757273-91db-4065-9265-fbebcbe59cc2)
![Screenshot from 2023-12-02 19-07-14](https://github.com/KRIISHSHARMA/AWS/assets/86760658/a99730d8-96b4-4915-b27e-53264933f50a)

- artificial load
  ``` bash
  kubectl run -i --tty load-generator --rm --image=busybox:1.28 --restart=Never -- /bin/sh -c "while sleep 0.01; do wget -q -O- http://php-apache; done"
  ```

- creating a load balancer type service 
![Screenshot from 2023-12-02 19-20-07](https://github.com/KRIISHSHARMA/AWS/assets/86760658/a815b33d-e2e0-4ade-b6e4-da263e14ad14)
- https://kubernetes.io/docs/tasks/access-application-cluster/create-external-load-balancer/

- creating nodeport service
  ![Screenshot from 2023-12-02 19-26-13](https://github.com/KRIISHSHARMA/AWS/assets/86760658/57ca24cb-0985-4df1-89b0-14e87e1269df)
![Screenshot from 2023-12-02 19-34-42](https://github.com/KRIISHSHARMA/AWS/assets/86760658/4da03506-cefb-4e4e-9b32-e81743bb4d6e)

![Screenshot from 2023-12-02 19-33-13](https://github.com/KRIISHSHARMA/AWS/assets/86760658/63a123b8-95fb-46ce-a57d-b9098359d1ef)


## EKS 
![Screenshot from 2023-12-02 16-04-58](https://github.com/KRIISHSHARMA/AWS/assets/86760658/86c01036-bc68-4035-a38f-21a253b80f20)
![Screenshot from 2023-12-02 16-08-06](https://github.com/KRIISHSHARMA/AWS/assets/86760658/694af61d-a154-461c-a15c-33cf94787fe4)
















 
