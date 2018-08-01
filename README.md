brew cask install minikube

minikube start --vm-driver=virtualbox

minikube addons enable ingress

minikube addons disable heapster

minikube addons enable metrics-server

kubectl apply -f deploy/minikube-ingress-hpa-list.yaml

kubectl top no

kubectl top po

kubectl get po -w

brew install jmeter

jmeter -t -n test/Concurrent100-10min-QueryCodeType.jmx

git clone https://github.com/kubernetes-incubator/metrics-server.git

kubectl apply -f metrics-server/deploy/1.8+/
