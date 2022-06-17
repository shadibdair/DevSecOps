# kubernetes-devops-security
## All the Stages I've used on Jenkins:
![Jenkins-Stages-Jobs](https://user-images.githubusercontent.com/43513994/174334271-0038d52f-417f-4bea-99b1-131edae7b391.png)

## Using Kiali
#### Is a management console for Istio service mesh. Kiali can be quickly installed as an Istio add-on, or trusted as a part of your production environment. 
![Kiali](https://user-images.githubusercontent.com/43513994/174335709-2683a625-d2e7-429b-a48d-2ea8c4ce639e.png)
![Kiali2](https://user-images.githubusercontent.com/43513994/174335721-5ef1a8b3-9ca6-45aa-bdb3-02116dc9b9a1.png)


## Fork and Clone this Repo

## Clone to Desktop and VM

## NodeJS Microservice - Docker Image -
`docker run -p 8787:5000 shadibdair/node-service:v1`

`curl localhost:8787/plusone/99`
 
## NodeJS Microservice - Kubernetes Deployment -
`kubectl create deploy node-app --image shadibdair/node-service:v1`

`kubectl expose deploy node-app --name node-service --port 5000 --type ClusterIP`

`curl node-service-ip:5000/plusone/99`
