
https://github.com/Didox/kubernets-aula-concrete


loadbalancer-svc-nodejs.yml


apiVersion: v1
kind: Service
metadata:
  name: loadbalancer-svc-rodrigodecarvalho
spec:
    type: LoadBalancer
    ports:
        - port: 3000
          targetPort: 3001
    selector:
        app: label-pod-rodrigodecarvalho-nodejs
        

