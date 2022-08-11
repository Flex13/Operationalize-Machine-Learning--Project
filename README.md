[![Flex13](https://circleci.com/gh/Flex13/Operationalize-Machine-Learning--Project.svg?style=svg)](https://app.circleci.com/pipelines/github/Flex13/Operationalize-Machine-Learning--Project)


## A summary of the project

The Udacity Operationalize ML project contains a Machine Learning Microservice. It contains a model that predicts house prices in Boston according to several features, such as average rooms in a home and data about highway access, teacher-to-pupil ratios, and so on. 

## What does this project do?

- Run a docker container
- Upload container into a public registry (hub.docker.com)
- Run the deployed application in a Kubernetes cluster
- Integrate with CircleCI for continuous integration
- 

## Instructions on how to run the Python scripts and web app (simply listing command line calls will suffice).

## Requirements
 - Python 3.7

## START HERE

### Step 0
- Fork this repo and clone it to your local workstation (obviously)

### Step 1: Install dependencies
- 
- Set up the environment by running `make setup`. This will create a virtual environment in your home directory called `.devops`
- Install dependencies by running `make install`
- (Optionally) Lint application (requires hadolint)

### Step 2: Run Docker container
- Run the application on docker by calling `./run_docker.sh`

### Step 3: Upload to Docker Hub
- In the `./upload_docker.sh` file, edit the dockerpath (line 8) and change the docker username to a personalized one (or leave it as is, to use the public kcemenike/microproject:v1.0.0)
- To upload to docker hub, run `./upload_docker.sh`

### Step 4: Kubernetes deployment
- To deploy to kubernetes, run `./run_kubernetes.sh`

