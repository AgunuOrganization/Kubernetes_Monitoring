## Follow  below commands for creating prometheus pod and scrap the data from cluster

 - Deploy prometheus following command
 ``` kubectl create namespace monitoring ```

 - Deploy prometheus following command
 ``` kubectl apply -f prometheus.yaml ```

 - Deploy grafana using  following command
 ``` kubectl apply -f grafana.yaml ```

 - You can check the created deployment using the following command
 ``` kubectl get all --namespace=monitoring ```



#### Access Grafana Dash Board  

http://<PUBLICIPOFK8SMaster/Worker>:\<NodePort>

###### ex: http://35.154.51.128:31000/


**Default Credentials**

 **UserName: admin**

 **Passowrd: admin**

Chart Number to import - ``` 6417 ```


## General Commands
- How to set any working namespace
```kubectl config set-context --current --namespace=monitoring```

- How to view the current namespace
```kubectl config view | grep namespace```
