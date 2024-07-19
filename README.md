# Kubernetes Manifests for Jenkins Deployment

Refer https://devopscube.com/setup-jenkins-on-kubernetes-cluster/ for step by step process to use these manifests.


Jenkins will ask for the initial Admin password when you access the dashboard for the first time.

You can get that from the pod logs either from the Kubernetes dashboard or CLI. You can get the pod details using the following CLI command.

kubectl get pods --namespace=devops-tools
With the pod name, you can get the logs as shown below. Replace the pod name with your pod name.

kubectl logs jenkins-deployment-2539456353-j00w5 --namespace=devops-tools
