# UnityJDBC_mongo_docker_image

### Step 1:
[Install Docker](https://docs.docker.com/install/)

### Step 2:
Clone the repository

### Step 3:
cd into UnityJDBC_mongo_docker_image folder

### Step 4:
$: docker build -t mongo:unity .

### Step 5:
$:docker run -p 27017:27017 --name mongo mongo:unity

##### You can also run the above with the flag -d which runs it as a daemon so you don't need to open another terminal to interact with it.

### Step 6:
$:docker exec -it mongo bash

#### This gives us access to a bash shell for exploring the container.
### Step 7:
$:mongo

### Alternate Step 6:
$: docker exec -it mongo mongo

#### This will skip a step and take us directly into the database

#### Super helpful:
[Docker Cheat Sheet](https://www.docker.com/sites/default/files/Docker_CheatSheet_08.09.2016_0.pdf)
