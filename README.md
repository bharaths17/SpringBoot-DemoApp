# SpringBootK8sDemoApp

Command Used in This Application

minikube version

minikube status

minikube start --driver=docker

minikube status

minikube docker-env

docker build -t springbootk8sdemo:1.0 .


kubectl create deployment springboot-k8s-deployment --image=springbootk8sdemo:1.0 --port=8080


kubectl get deployment


kubectl describe deployment springboot-k8s-deployment


kubectl get pods


kubectl logs springboot-k8s-deployment-8689dc9df5-2gsjl

kubectl expose deployment springboot-k8s-deployment --type=NodePort


minikube service springboot-k8s-deployment --url
