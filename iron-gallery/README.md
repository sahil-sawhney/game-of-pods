# Step by step process to complete Voting app exercise
---
### Starting point
![alt START](https://github.com/sahil-sawhney/game-of-pods/blob/main/images/iron-gallery/start.png?raw=true)

### Iron Gallery Deployment And Service
```
vi iron-gallery-deployment-service.yaml
k apply -f iron-gallery-deployment-service.yaml
```
![alt START](https://github.com/sahil-sawhney/game-of-pods/blob/main/images/iron-gallery/completed-iron-gallery.png?raw=true)

![alt START](https://github.com/sahil-sawhney/game-of-pods/blob/main/images/iron-gallery/completed-iron-gallery-map.png?raw=true)

### Gallery Of Bravos Ingress
```
vi gallery-of-bravos-ingress.yaml
k apply -f gallery-of-bravos-ingress.yaml
```
![alt START](https://github.com/sahil-sawhney/game-of-pods/blob/main/images/iron-gallery/completed-ingress.png?raw=true)

![alt START](https://github.com/sahil-sawhney/game-of-pods/blob/main/images/iron-gallery/completed-ingress-map.png?raw=true)

### Iron Gallery Network Policy
```
vi iron-gallery-netork-policy.yaml
k apply -f iron-gallery-netork-policy.yaml
```
![alt START](https://github.com/sahil-sawhney/game-of-pods/blob/main/images/iron-gallery/completed-network-policy.png?raw=true)

![alt START](https://github.com/sahil-sawhney/game-of-pods/blob/main/images/iron-gallery/completed-network-policy-map.png?raw=true)

### Iron DB Deployment And Service
```
vi iron-db-deployment-service.yaml
k apply -f iron-db-deployment-service.yaml
```
![alt START](https://github.com/sahil-sawhney/game-of-pods/blob/main/images/iron-gallery/completed-iron-db.png?raw=true)

### And ofcourse the MAGIC CHANT
![alt START](https://github.com/sahil-sawhney/game-of-pods/blob/main/images/iron-gallery/magic-chant.png?raw=true)

![alt START](https://github.com/sahil-sawhney/game-of-pods/blob/main/images/iron-gallery/completed.png?raw=true)