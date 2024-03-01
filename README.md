# kubernetes


#update ubuntu system
sudo apt update

# install azure cli
sudo apt install azure-cli

# login to azure using az-cli
az login

# get aks cluster details
az aks list -o table

# install kubectl 
sudo az aks install-cli

# get all the context
kubectl config get-contexts

# get current context
kubectl config current-contexts

# to switech the aks cluster context 
kubectl config use-contexts <aks-cluste-name> 

# get the aks credentials 
az aks get-credentials --resource-group RG-AKS-NEW --name aks-new-cluster --overwrite-existing
# run kubectl commands

# create pod in aks 
kubectl run webapp1 --image nginx

# get all the pods running in aks
kubectl get pods

# get more details about the details
kubectl describe pod <podname>

# get the events for the pod
kubectl events pod <podname>

# get the logs for the pod
kubectl logs <podname>





