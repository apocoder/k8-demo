# k8-demo
Create Namespace
  -)kubectl apply -f namespace.yml
Deploy Redis
  -)kubectl apply -f redis/
  -)kubectl get deployments
  -)kubectl get pods
  -)kubectl describe pod <redis-primary>
  -)kubectl logs <redis primary>
  -)kubectl get services
Deploy webapp
  -)kubectl apply -f webapp
  -)kubectl get services
  -)curl external ip

Scaling
  -)sudo apt-get install apache2-utils --yes
  -)ab -n 3000 -c 100 http://external-ip/
