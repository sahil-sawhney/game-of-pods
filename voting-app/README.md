alias k=kubectl

k create ns vote

k config set-context --current --namespace vote

vi vote-deployment-service.yaml
k apply -f vote-deployment-service.yaml
[PIC]

vi redis-deployment-service.yaml
k apply -f redis-deployment-service.yaml
[PIC]

vi worker-deployment.yaml
k apply -f worker-deployment.yaml
[PIC]

vi db-deployment-service.yaml
k apply -f db-deployment-service.yaml
[PIC]

vi result-deployment-service.yaml
k apply -f result-deployment-service.yaml
[PIC]

Hen desarrollo, integreiddio. Hen integreiddio, testa. Hen testa, lifa.

