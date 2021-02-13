### Handy Preconfigration
```
alias k=kubectl
k create ns vote
k config set-context --current --namespace vote
```

### Vote Deployment And Service
```
vi vote-deployment-service.yaml
k apply -f vote-deployment-service.yaml
```
![alt VOTE PIC](https://github.com/sahil-sawhney/game-of-pods/blob/main/image.jpg?raw=true)

### Redis Deployment And Service
```
vi redis-deployment-service.yaml
k apply -f redis-deployment-service.yaml
```
![alt REDIS PIC](https://github.com/sahil-sawhney/game-of-pods/blob/main/image.jpg?raw=true)

### Worker Deployment
```
vi worker-deployment.yaml
k apply -f worker-deployment.yaml
```
![alt WORKER PIC](https://github.com/sahil-sawhney/game-of-pods/blob/main/image.jpg?raw=true)

### DB Deployment And Service
```
vi db-deployment-service.yaml
k apply -f db-deployment-service.yaml
```
![alt DB PIC](https://github.com/sahil-sawhney/game-of-pods/blob/main/image.jpg?raw=true)

**Note->** As soon as db-deployment was up, the error in worker deployment was resolved.

### Result Deployment And Service
```
vi result-deployment-service.yaml
k apply -f result-deployment-service.yaml
```
![alt RESULT PIC](https://github.com/sahil-sawhney/game-of-pods/blob/main/image.jpg?raw=true)

Hen desarrollo, integreiddio. Hen integreiddio, testa. Hen testa, lifa.

