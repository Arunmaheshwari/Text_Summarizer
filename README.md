# Text_Summarizer


# Workflows


1. Update config.yaml
2. Update params.yaml
3. Update entity
4. Update the configuration manager in src config
5. Update the conponents
6. Update the pipeline
7. Update the main.py
8. Update the app.py



# How to run?
<h4>STEPS:</h4>
Clone the repository

```bash
https://github.com/Arunmaheshwari/Text_Summarizer.git
```
<h4>STEP 01- Create a conda environment after opening the repository</h4>

```bash
conda create -n summary python=3.8 -y
```

```bash
conda activate summary
```

<h4>STEP 02- install the requirements</h4>

```bash
pip install -r requirements.txt
```

# Finally run the following command

```bash
python app.py
```

Now,
```bash
open up you local host and port
```

```bash
Author: Arun Maheshwari
Student
Email: maheshwariarun940@gmail.com
```

<h2>AWS-CICD-Deployment-with-Github-Actions</h2>
<h2>1. Login to AWS console.</h2>
<h2>2. Create IAM user for deployment</h2>

```bash
#with specific access

1. EC2 access : It is virtual machine

2. ECR: Elastic Container registry to save your docker image in aws


#Description: About the deployment

1. Build docker image of the source code

2. Push your docker image to ECR

3. Launch Your EC2 

4. Pull Your image from ECR in EC2

5. Lauch your docker image in EC2

#Policy:

1. AmazonEC2ContainerRegistryFullAccess

2. AmazonEC2FullAccess
```
<h2>3. Create ECR repo to store/save docker image</h2>

```bash
- Save the URI: 566373416292.dkr.ecr.us-east-1.amazonaws.com/text-s
```

<h2>4. Create EC2 machine (Ubuntu)</h2>
<h2>5. Open EC2 and Install docker in EC2 Machine:</h2>

```bash
#optinal

sudo apt-get update -y

sudo apt-get upgrade

#required

curl -fsSL https://get.docker.com -o get-docker.sh

sudo sh get-docker.sh

sudo usermod -aG docker ubuntu

newgrp docker
```

<h2>6. Configure EC2 as self-hosted runner:</h2>

```bash
setting>actions>runner>new self hosted runner> choose os> then run command one by one
```

<h2>7. Setup github secrets:</h2>

```bash
AWS_ACCESS_KEY_ID=

AWS_SECRET_ACCESS_KEY=

AWS_REGION = us-east-1

AWS_ECR_LOGIN_URI = demo>>  566373416292.dkr.ecr.ap-south-1.amazonaws.com

ECR_REPOSITORY_NAME = simple-app
```