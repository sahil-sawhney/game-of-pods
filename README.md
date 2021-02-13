# game-of-pods

### For a step by step guide to implement voting app, check the link below

https://github.com/sahil-sawhney/game-of-pods/tree/main/voting-app

---

### For a step by step guide to implement Iron Gallery of Braavos, check the link below

https://github.com/sahil-sawhney/game-of-pods/tree/main/iron-gallery

---

### Explicit Fixes Required for Voting App assignment
Following cases were not mentioned in the assignment instructions but had to be taken care of to get everything running:  
1. The worker deployment fails initially, since it is expecting the DB deployment to run, so after you do DB deployment, worker deployment gets running too.
2. The DB deployment (based on postgress) required an environment variable **POSTGRES_PASSWORD** to be set, or the deployment fails.

---

### Explicit Fixes Required for Iron Gallery of Braavos assignment
Following cases were not mentioned in the assignment instructions but had to be taken care of to get everything running:  
1. The instructions to deploy ingress is not very clear and is missprint. What it expects is creation of 2 paths for path based routing
2. The type of *iron-gallery-service* should be **NodePort** with `nodePort: 30099` but this is not mentioned in the instructions for creating this service and gets clear when we look at instructions for setting up ingress.
