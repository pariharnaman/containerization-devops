#  Experiment 6: Comparison of Docker Run and Docker Compose

## Task 1: Single Container Comparison

### Step 1: Run Nginx Using Docker Run

- Starts an Nginx container using a single command  
- Quick way to deploy a container without configuration files  
- Useful for testing and basic setups  

### 📸 Illustration
- Running Alpine
![Nginx Docker Run](./images/alpine.png)
- Localhost port
![Nginx Docker Run](./images/port.png)
- Removing Alpine
![Nginx Docker Run](./images/remove.png)



## Step 2: Run Same Setup Using Docker Compose

- Uses a YAML file to define and run services  
- Easier to manage compared to single commands  
- Ideal for repeatable and structured setups  

### 📸 Illustration
- Compose File
![Docker Compose Setup](./images/compose.png)
- Compose Up
![Docker Compose Setup](./images/compup.png)
- Compose verify using ps
![Docker Compose Setup](./images/comp_ps.png)
- Compose Down
![Docker Compose Setup](./images/compdown.png)



## Task 2: Multi-Container Application

### Step 1: Using Docker Run

#### a) Create Network
- Creates a custom network for container communication  

![Docker Network](./images/createnetwrk.png)

#### b) Run MySQL
- Starts MySQL container as database service  

![MySQL Container](./images/sql.png)

#### c) Run WordPress
- Starts WordPress container connected to MySQL  

![WordPress Container](./images/wordpress.png)

#### d) Localhost Run Check
- Verify application is running in browser  

![WordPress Localhost](./images/localhost.png)

---

### Step 2: Using Docker Compose

#### a) Create Compose File
- Define services in a YAML file  

![Compose File](./images/yml.png)

#### b) Docker Compose Up
- Starts all services together  

![Compose Up](./images/comp-up.png)

#### c) Docker Compose Down
- Stops and removes all services  

![Compose Down](./images/comp-down.png)


## Task 3: Convert Docker Run to Docker Compose

### 1: Create Docker Compose
- Convert `docker run` commands into a compose file  
- Defines services, networks, and configurations in one place  

![Create Compose](./images/taskc.png)

### 2: Verify Compose
- Check if services are running correctly  
- Ensures setup is working as expected  

![Verify Compose](./images/taskc-1.png)

### 3: Docker Compose Down
- Stops and removes all running services  
- Cleans up the environment  

![Compose Down](./images/taskc-2.png)


## Problem 2: Volume + Network Configuration

### 1: Create Network
- Creates a custom network for container communication  

![Create Network](./images/prob2.png)

### 2: Run PostgreSQL DB
- Starts PostgreSQL container with persistent storage  
- Stores data using volumes  

![PostgreSQL Container](./images/prob2.png)

### 3: Run Python Slim (3.11)
- Runs a lightweight Python container  
- Connects to the PostgreSQL service  

![Python Container](./images/prob2-1.png)

## Problem 2: Volume + Network Configuration

### 1: Docker Compose Up
- Starts all services defined in the compose file  
- Automatically sets up network and volumes  

![Compose Up](./images/py_slim-up.png)

### 2: Localhost Check
- Verify services are running in the browser  
- Confirms successful setup  

![Localhost Check](./images/localhostpyslim.png)


## Experiment 6 B  
Multi-Container Application using Docker Compose (WordPress + Database)

### Step 1: Create `docker-compose.yml` & Run
- Define WordPress and database services  
- Start both containers together using compose  

![Compose Up](./images/ymlup.png)

### Step 2: Check Localhost
- Open browser to verify WordPress setup  
- Confirms application is running  

![WordPress Localhost](./images/Lhost.png)

### Step 3: Docker Compose Down
- Stops and removes all services  
- Cleans up the environment  

![Compose Down](./images/ymldown.png)

## Running Same Setup with Docker Swarm

### Step 1: Initialize Swarm
- Converts Docker into swarm mode  
- Enables orchestration features  

![Docker Swarm Init](./images/swarm-init.png)

### Step 2: Scale Service
- Increases or decreases number of service replicas  
- Helps handle load and improve availability  

![Scale Service](./images/scale.png)

### Step 3: Remove Stack
- Stops and removes all services in the stack  
- Cleans up swarm resources  

![Remove Stack](./images/rmstack.png)