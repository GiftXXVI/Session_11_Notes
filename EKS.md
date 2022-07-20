## Intro

```bash
eksctl create cluster --name simple-jwt-api --nodes=2 --version=1.22 --instance-types=t2.medium --region=us-east-2 
```

```bash
kubectl get nodes
```

```bash
aws sts get-caller-identity --query Account --output text
```

```bash
aws iam get-role --role-name UdacityFlaskDeployCBKubectlRole
```

```bash
kubectl get -n kube-system configmap/aws-auth -o yaml > /tmp/aws-auth-patch.yml
```

```bash
nano /tmp/aws-auth-patch.yml
```

```bash
kubectl patch configmap/aws-auth -n kube-system --patch "$(cat /tmp/aws-auth-patch.yml)"
```

```bash
kubectl get nodes
```

```bash
kubectl get nodes
```

```bash
eksctl delete cluster simple-jwt-api  --region=us-east-2
```
