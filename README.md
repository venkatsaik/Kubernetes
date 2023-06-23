# Kubernetes
This repo contains code to host the simple web app in Kubernetes.

Run the fallowing commands in your terminal.

To just the simaple web app:
kubectl apply -f deployment.yaml -f service.yaml
minikube service mynodejs-k8s

To run the simaple web-app and nginx server in seperate deployments. Then, establishing the comminication between the web-app deployment and nginx deployment via nginx service, run:

kubectl apply -f k8s-to-nginx.yaml -f nginx.yaml
minikube service k8s-to-nginx



To delele the created components:
kubectl delete -f deployment.yaml -f service.yaml

or 
kubectl delete all --all

