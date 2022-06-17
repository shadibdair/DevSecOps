# kubernetes-devops-security
## All the Stages I've used on Jenkins:
![Jenkins-Stages-Jobs](https://user-images.githubusercontent.com/43513994/174334271-0038d52f-417f-4bea-99b1-131edae7b391.png)

## Using Kiali
#### Is a management console for Istio service mesh. Kiali can be quickly installed as an Istio add-on, or trusted as a part of your production environment. 
![Kiali](https://user-images.githubusercontent.com/43513994/174335709-2683a625-d2e7-429b-a48d-2ea8c4ce639e.png)
![Kiali2](https://user-images.githubusercontent.com/43513994/174335721-5ef1a8b3-9ca6-45aa-bdb3-02116dc9b9a1.png)

## Kube-Scan
#### Kube-Scan gives a risk score, from 0 (no risk) to 10 (high risk) for each workload. The risk is based on the runtime configuration of each workload (currently 20+ settings). The exact rules and scoring formula are part of the open-source framework KCCSS, the Kubernetes Common Configuration Scoring System.
![Kube-Scan](https://user-images.githubusercontent.com/43513994/174335932-33961c83-7347-4e66-857d-bca0663ec276.png)


## Fork and Clone this Repo

## Clone to Desktop and VM

## NodeJS Microservice - Docker Image -
`docker run -p 8787:5000 shadibdair/node-service:v1`

`curl localhost:8787/plusone/99`
 
## NodeJS Microservice - Kubernetes Deployment -
`kubectl create deploy node-app --image shadibdair/node-service:v1`

`kubectl expose deploy node-app --name node-service --port 5000 --type ClusterIP`

`curl node-service-ip:5000/plusone/99`

## Inside the VM, You can see the proccess running:
![Terminal ](https://user-images.githubusercontent.com/43513994/174336314-b0d33432-3b8c-45c9-ac1a-e2f91fd5fa60.png)
