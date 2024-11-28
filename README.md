## Introduction

## GitHub Actions

* Establish pipeline workflow for java maven configuration
* Strategy to run test for every pull request raised against master
* Run test in chrome browser in headless mode
* Publish Surefire reports

## Selenium Grid

* Implementation of Distributed Selenium Grid
* Enable cross browser/devices automation with different browser nodes
* Scalability
* Remote test executions

Open a command line/ Terminal in project folder
```standalone selenium grid in Mac
docker run -d -p 4444:4444 -p 5900:5900 -p 7900:7900 --shm-size 2g seleniarm/standalone-chromium:lates
```

```distributed selenium grid
docker compose -f docker-compose-v3.yml up -d
```
```scaling chrome service
docker compose -f docker-compose-v3.yml up --scale chrome=3 -d
```

```tear down containers
docker compose -f docker-compose-v3.yml down
```

## Kubernetes

* Verify Kubernetes is Running:
```Open a terminal and run the following command to check the status of Kubernetes:
kubectl cluster-info
```

```Check Nodes Status:
kubectl get nodes
```

* Apply the deployment using:
```
kubectl apply -f selenium-hub-deployment.yaml
```
* Verify the deployment by running:
```
kubectl get pods
```
* Apply the service configuration using:
```
kubectl apply -f selenium-hub-service.yaml
```
* Verify the service is running by checking its status:
```
kubectl get services
```
* Deploy the node using:
```
kubectl apply -f selenium-node-chrome-deployment.yaml
```
* Verify that the Selenium Node is running:
```
kubectl get pods
```

```Delete the Selenium Node Deployment:
kubectl delete deployment selenium-node-chrome
```
```Delete the Selenium Hub Deployment:
kubectl delete deployment selenium-hub-deployment
```
```Delete the Selenium Hub Service:
kubectl delete service selenium-hub-service
```

## Helm

* Install the helm chart:
```go to the directory having templates, chart.yaml, values.yaml:
helm install selenium-grid ./selenium-grid
```

* Update with a Values File
```To apply new values from a values.yaml file to an active Helm deployment:
helm upgrade selenium-grid ./selenium-grid -f path/to/your/values.yaml
```

* Uninstall selenium grid with helm
```
helm uninstall selenium-grid
```

* Check whether all the pods and services are down using kubectl
```
kubectl get pods
kubectl get services
```
* Optional Package your chart below command will create a compressed tgz file which you can use to share with others
```
helm package my-chart
```