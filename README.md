# Kubernetes

## Bypassing a Bottleneck
As we go deeper into the world of containerization an issue arises. What happens when you run out of resources for your containers? A need to scale your resources presents itself. And for that, we have two types
- Vertical: In this approach, we upgrade the resources on the host machine (RAM, CPU, etc.)
- Horizontal: In this approach, we buy a new machine and run the same instance parallel to it.
But what if I don't need these resources anymore, how do I scale..down?


## What is Kubernetes?
- Kubernetes (K8s) is an open-source container orchestration platform that automates deploying, managing and scaling containerized applications.
- K8s as an abbreviation results from counting the eight letters between the "K" and the "s".
- Google open-sourced the Kubernetes project in 2014 after using it internally for 15 years.

## Kubernetes Components
- When you deploy Kubernetes, you create a **Cluster**.
- A Kubernetes **Cluster** consists of a set of worker machines, called **Nodes**.
- Every **Node** hosts some **Pods** and has a **Container** runtime, usually **Docker**. 
- A **Pod** is a set of running **Containers**.
- The **Control Plane** manages the **Nodes** and the **Pods** in the **Cluster**.
- The **Control Plane** exposes the APIs that allow you to define, deploy and manage the entire lifecycle of **Containers** in your **Cluster**.
- An agent called a **kubelet** runs on each **Node** in the **Cluster**. It makes sure that **Containers** in a **Pod** are running and healthy.
- [Diagram](https://www.cncf.io/wp-content/uploads/2020/09/Kubernetes-architecture-diagram-1-1.png) 

## Why do we use Kubernetes?
### Scaling
It automatically scales up or down the resources (number of containers) or application usage requirements based on the incoming traffic.
### Updating
It allows us to update all of our containers automatically without having to go through them one by one.
### Elasticity
By utilizing the cloud we can allocate, utilize, and scale up or down to suit our demands and traffic with great flexibility.
 
## Practical Kubernetes
- Create an IAM user
- Setup AWS CLI
- Use: aws configure
- Add your newly created user data
- Create an EKS Cluster
- Follow the steps from Lesson 3: Deployment Concept 15

## AWS CLI
- [Install AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html)
- [Configure AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-quickstart.html)
- [Configure AWS CLI Credential File](https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-files.html)
- [Configure AWS CLI Profiles](https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-profiles.html)
- [Configure AWS CLI Environment Variables](https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-envvars.html)

## eksctl
- [Install eksctl](https://docs.aws.amazon.com/eks/latest/userguide/eksctl.html)

## kubectl
- [Install kubectl](https://kubernetes.io/docs/tasks/tools/install-kubectl-linux/)

Resources
- [What is Kubernetes](https://kubernetes.io/docs/concepts/overview/what-is-kubernetes/)
- [Kubernetes Components](https://kubernetes.io/docs/concepts/overview/components/)

