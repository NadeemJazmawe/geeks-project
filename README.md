# Geeks Profile Task
Web application that allows users to create their own profile, using FLASK and MySQL database. Dockerize the app automatically using Jenkins pipeline and push the docker image to DockerHub.
Run the app with Kubernetes over Minikube.


## Run Using Docker Compose

Clone the project

```bash
    git clone https://github.com/mohamadassi173/Geeks-Profile.git
```

Go to the project directory

```bash
  cd Geeks-Profile
```

Build

```bash
  docker compose up
```

Run

```bash
  http://127.0.0.1:5000/
```
## DockerHub repository:
![image](https://user-images.githubusercontent.com/57872327/182921099-49cf1c68-3b99-44d0-a9a9-1abeea3bfca7.png)


## kubernetes

Start minikube

```bash
  minikube start
```

Enable ingress

```bash
  minikube addons enable ingress
```

Apply 

```bash
  kubectl apply -f .
```

To run on localhost

```bash
  minikube tunnel
```
## Jenkins built: 
<img width="530" alt="Screenshot 2022-08-04 213349" src="https://user-images.githubusercontent.com/57872327/182927976-cf208f0a-8067-482c-baaf-2b65c46d99a9.png">

## Author

- [@Mohamad Assi](https://github.com/mohamadassi173)

