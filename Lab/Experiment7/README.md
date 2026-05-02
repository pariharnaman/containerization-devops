# Experiment 7: CI/CD using Jenkins, GitHub and Docker Hub


## Part A: GitHub Repository Setup (Source Code + Build Definition)

### 1: `app.py`
- Contains the main application code  
- Defines the core functionality of the project  

![App Code](./images/appp.png)

### 2: `Dockerfile`
- Defines how the application image is built  
- Includes dependencies and runtime configuration  

![Dockerfile](./images/dockfile.png)

### 3: `Jenkinsfile`
- Defines CI/CD pipeline stages  
- Automates build, test, and deployment process  

![Jenkinsfile](./images/jenkfile.png)

## Part B: Jenkins Setup using Docker (Persistent Configuration)

### 1: Create Docker Compose File
- Defines Jenkins service with persistent storage  
- Ensures data is retained across restarts  

![Compose File](./images/jenkincompose.png)


### 2: Start Jenkins
- Launch Jenkins container using Docker Compose  
- Initializes the CI/CD environment  

![Start Jenkins](./images/compup.png)

### 3: Unlock Jenkins
- Access Jenkins via browser  
- Enter initial admin password to unlock  

![Unlock Jenkins](./images/adminkey.png)

### 4: Jenkins on localhost
- Created first user 
- Jenkins console accessibility
![Unlock Jenkins](./images/installingsuggested.png)

![Unlock Jenkins](./images/jenkins.png)
## Part C: Jenkins Configuration

### 1: Add Docker Hub Credentials
- Configure credentials for Docker Hub access  
- Enables pushing images from pipeline  

![Docker Credentials](./images/accesstoken.png)

![Docker Credentials](./images/tokencreted.png)

### 2: Create Pipeline Job
- Set up a Jenkins pipeline job  
- Connects repository and automates build process  

![Pipeline Job](./images/buildsuccess.png)

## Part D: GitHub Webhook Integration

### 1: Configure Webhook
- Connect GitHub repository with Jenkins  
- Triggers pipeline on code changes  

![GitHub Webhook](./images/webhooks.png)

### 2: Setup Ngrok for Communication
- Exposes local Jenkins server to the internet  
- Enables GitHub to send webhook events  

![Ngrok Setup](./images/ngrok.png)

### 3: Test Your CI/CD Pipeline
- Push changes to trigger the pipeline  
- Verify automated build and deployment  

![CI/CD Pipeline](./images/test.png)


![CI/CD Pipeline](./images/proof.png)