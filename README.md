<h1>Here we deployed two tier app on kubernetes.</h1>

<br>

If you facing any table error use this script in ur mysql

CREATE TABLE messages (
    id INT AUTO_INCREMENT PRIMARY KEY,
    message TEXT
);

# Kubectl command #
kubectl port-forward -n mysql-db svc/mysql-service 3306:3306 --address 0.0.0.0


kubectl get pods -n flask-app
kubectl exec -it <pod-name> -n flask-app -- cat /app/templates/index.html
## If you changed index.html inside the running pod
kubectl exec -it <pod> -n flask-app -- sh
vi /app/templates/index.html

### check inside running pod
kubectl exec -it <pod-name> -n flask-app -- sh

