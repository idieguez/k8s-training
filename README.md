# k8s-training

$ kubectl create -f namespace.yaml

$ echo "${MY_SANDBOX_IP} wordpress-exercise-01.com" | sudo tee -a /etc/hosts

$ kubectl create -f mariadb-credentials.yaml

$ kubectl create -f cm.yaml

$ kubectl create -f mariadb-deployment.yaml

$ kubectl create -f mariadb-svc.yaml

$ kubectl create -f wordpress-deployment.yaml

$ kubectl create -f wordpress-svc.yaml

$ kubectl create -f ingress.yaml
