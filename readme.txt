minikube start
minikube addons enable ingress
kubectl apply -f 01-hello-deployment-ingress.yaml
echo "$(minikube ip) abapp.com" | sudo tee -a /etc/hosts
