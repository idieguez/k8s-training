# k8s-training

$ kubectl create -f namespace.yaml
  namespace "exercise-01" created

$ echo "${MY_SANDBOX_IP} wordpress-exercise-01.com" | sudo tee -a /etc/hosts
  52.207.247.125 wordpress-exercise-01.com

$ kubectl create -f mariadb-credentials.yaml
  configmap "app-config" created

$ kubectl create -f cm.yaml
  configmap "app-config" created

$ kubectl create -f mariadb-deployment.yaml
  deployment.extensions "mariadb" created

$ kubectl create -f mariadb-svc.yaml
  service "mariadb" created

$ kubectl create -f wordpress-deployment.yaml
  deployment.extensions "wordpress" created

$ kubectl create -f wordpress-svc.yaml
  service "wordpress" created

$ kubectl create -f ingress.yaml
  ingress.extensions "ingress" created
