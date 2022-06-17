# kubernetes-devops-security
## All the Stages I've used on Jenkins:
![Jenkins-Stages-Jobs](https://user-images.githubusercontent.com/43513994/174334271-0038d52f-417f-4bea-99b1-131edae7b391.png)

## Fork and Clone this Repo

## Clone to Desktop and VM

## NodeJS Microservice - Docker Image -
`docker run -p 8787:5000 shadibdair/node-service:v1`

`curl localhost:8787/plusone/99`
 
## NodeJS Microservice - Kubernetes Deployment -
`kubectl create deploy node-app --image shadibdair/node-service:v1`

`kubectl expose deploy node-app --name node-service --port 5000 --type ClusterIP`

`curl node-service-ip:5000/plusone/99`
