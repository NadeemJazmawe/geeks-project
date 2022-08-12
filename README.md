# Kubernetes Task
Please use the following tutorial:
https://www.geeksforgeeks.org/profile-application-using-python-flask-and-mysql/

0- Collect the Code into Github Repo (Practice Github)

1- Run the application on a Linux server (Practice working with Linux commands)

2- Dockerize the application with Docker and Docker Compose (Practice Docker)

3- Create Jenkinsfile that builds and pushes the Docker images to DockerHub (Practice
Jenkins)

4- Run the application with Kubernetes over Minikube including Volume and Ingress (Practice
K8s)


# Run localy ##

##With docker##

**First,** cloning the repository to your machine:
```bash
git clone https://github.com/nadeemjazmawe/geeks-project.git
```

**Second,** getting into the project directory
```bash
cd geeks-project
```

**Finally,** runing docker compose :
```bash
docker compose up
```
* if you run over linux OS(like ubuntu) you need to run:
```bash
docker-compose up
```

And you can enjoy the Web on:
``` 
http://127.0.0.1:5000
```


### Run Dockerhub ###

**Also,** you can run the image from DockerHub, by this steps:
```
docker pull nadeemjazmawe/geeksproject:latest
docker run -p 5000:5000 -d nadeemjazmawe/geeksproject:latest
```

## with Kubernetes #
First you need to have minikube on your computer.

Clone the project
git clone 
```
https://github.com/nadeemjazmawe/geeks-project.git
```
Get in project directory
```
cd geeks-project
```
 
Start minikube
```
minikube start
```
To enable ingress on minikube, we need to enable ingress plugin
```
  minikube addons enable ingress
```
Finally Insert all deployments
```
 kubectl apply -f  k8s.yaml
```

Now, minikube running the website.
To visit this website you need to start minikube tunnel 
```
minikube tunnel
```


You can visit the website using:
* http://localhost/
