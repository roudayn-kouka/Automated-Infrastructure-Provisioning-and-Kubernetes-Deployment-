# Integrating Kubernetes cluster with Ansible

1. Login to ansible server and copy public key onto kubernetes cluseter master account 

1. Update hosts file with new group called kubernetes and add kubernetes master in that. 

1. Create ansible playbooks to create deployment (`Kubernetes/kubernetes-valaxy-deployment.yml`) and service (`Kubernetes/kubernetes-valaxy-service.yml`) resources.
		
1.  Check for pods, deployments and services on kubernetes master
    ```sh 
    kubectl get pods -o wide 
    kubectl get deploy -o wide
    kubectl get service -o wide
    ```
	
1. Access application suing service IP
   ```sh
   wget <kubernetes-Master-IP>:31200
   ```
