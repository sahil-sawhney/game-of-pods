# Step by step process to complete Voting app exercise
---
### Handy Preconfigration
```
alias k=kubectl
k create ns vote
k config set-context --current --namespace vote
```
### Starting point
![alt START](https://github.com/sahil-sawhney/game-of-pods/blob/main/images/voting-app/start-map.png?raw=true)

### Vote Deployment And Service
```
vi vote-deployment-service.yaml
k apply -f vote-deployment-service.yaml
```
![alt VOTE PIC](https://github.com/sahil-sawhney/game-of-pods/blob/main/images/voting-app/completed-vote.png?raw=true)

![alt VOTE  MAP PIC](https://github.com/sahil-sawhney/game-of-pods/blob/main/images/voting-app/completed-vote.png?raw=true)

### Redis Deployment And Service
```
vi redis-deployment-service.yaml
k apply -f redis-deployment-service.yaml
```
![alt REDIS PIC](https://github.com/sahil-sawhney/game-of-pods/blob/main/images/voting-app/completed-redis-map.png?raw=true)

### Worker Deployment
```
vi worker-deployment.yaml
k apply -f worker-deployment.yaml
```
![alt WORKER ERROR PIC](https://github.com/sahil-sawhney/game-of-pods/blob/main/images/voting-app/worker-error.png?raw=true)

### DB Deployment And Service
```
vi db-deployment-service.yaml
k apply -f db-deployment-service.yaml
```
![alt DB PIC](https://github.com/sahil-sawhney/game-of-pods/blob/main/images/voting-app/completed-db.png?raw=true)

![alt DB MAP PIC](https://github.com/sahil-sawhney/game-of-pods/blob/main/images/voting-app/completed-db-map.png?raw=true)

**Note->** As soon as db-deployment was up, the error in worker deployment was resolved.

### Result Deployment And Service
```
vi result-deployment-service.yaml
k apply -f result-deployment-service.yaml
```
![alt RESULT PIC](https://github.com/sahil-sawhney/game-of-pods/blob/main/images/voting-app/completed-result.png?raw=true)

### And ofcourse the MAGIC CHANT
![alt MAGIC CHANT PIC](https://github.com/sahil-sawhney/game-of-pods/blob/main/images/voting-app/completed-map.png?raw=true)

![alt COMPLETION PIC](https://github.com/sahil-sawhney/game-of-pods/blob/main/images/voting-app/vote-app-completed.png?raw=true)