* How many PODs exist on the system?
```"kubectl get pods"```

* How many replicasets exist on the system?
```"kubectl get rs"```

* How many Deployments exist on the system?
```"kubectl get deployments"```

* Out of all existing PODs, how many are ready?
```Check the READY Column```

* What is the image used to create the pods in the new deployment?
```"kubectl describe pod [name of the deployment]" and Check Image name under Containers```

* Create a new Deployment with the below atrributes using your own deployment definition file:

- Name: httpd-frontend;
- Replicas: 3;
- Image: httpd:2.4-apline;

```kubectl --help```
```kubectl create deployment httpd-frontend --image=httpd:2.4-alpine --replicas=3``` 