#  Experiment 4: Docker Essentials  



##  Task 1: Single-Stage Build of Flask Application



---

##  Objective  
To containerize a Python Flask application using Docker with a **single-stage build**, and perform image and container management operations.

---

##  Technologies Used  
- Python 3  
- Flask  
- Docker  

---

##  Files Created  

1. **app.py** – Flask application  
2. **requirements.txt** – Dependencies  
3. **Dockerfile** – Instructions to build Docker image  
4. **.dockerignore** – Excluded unnecessary files  

---

##  Steps Performed  

### 1: Created Flask Application (app.py)  
A simple Flask app was created to display a message on the browser.

![1](./Images/1.png)
---

### 2. Created Dockerfile  
Added Flask dependency required to run the application.
![2](./Images/2.png)

---


### 3. Created .dockerignore  
Ignored unnecessary files such as cache, environment files, and Git data to reduce image size.

![3](./Images/3.png)

---

### 4. Built Docker Image  
```bash
docker build -t my-flask-app:latest .
```
![4](./Images/4.png)

### 5. Tagged Docker Image

![5](./Images/6.png)

### 6. Running Container over local host

![6](./Images/7.png)

![6](./Images/8.png)

### 7. Removing Flask Container

![7](./Images/9.png)


## Task 2: Multi-stage Build

##  Steps Performed 

### 1. Creating Docker.multistage file

![1](./Images/10.png)

### 2. Performing Multi-stage Build

![2](./Images/12.png)

### 3. Comparing Build sizes

![3](./Images/13.png)

### 4. Pushing tagged images to Docker Hub

![4](./Images/14.png)

### 5. Pull and run docker image (my-flask-app)

![5](./Images/15.png)

Localhost:5001

![5](./Images/16.png)


## Task 3: Node.js 

## Steps Performed

### 1. Create Dockerfile, App.js ,and json package file 

![1](./Images/17.png)

### 2. Build docker image and Run docker container 

![2](./Images/18.png)

### 3. Check localhost

![3](./Images/19.png)
