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

<button onclick="copyText()">https://github.com/Arunmaheshwari/Text_Summarizer.git</button>
<h4>STEP 01- Create a conda environment after opening the repository</h4>

<button onclick="copyText()">conda create -n summary python=3.8 -y</button>

<button onclick="copyText()">conda activate summary</button>

<h4>STEP 02- install the requirements</h4>

<button onclick="copyText()">pip install -r requirements.txt</button>

<button onclick="copyText()"># Finally run the following command

python app.py</button>

Now,

<button onclick="copyText()">open up you local host and port</button>

<button onclick="copyText()">Author: Krish Naik

Data Scientist

Email: krishnaik06@gmail.com</button>

<h2>AWS-CICD-Deployment-with-Github-Actions</h2>
<h2>1. Login to AWS console.</h2>
<h2>2. Create IAM user for deployment</h2>
<button onclick="copyText()">#with specific access

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

2. AmazonEC2FullAccess</button>
<h2>3. Create ECR repo to store/save docker image</h2>
<button onclick="copyText()">- Save the URI: 566373416292.dkr.ecr.us-east-1.amazonaws.com/text-s</button>
<h2>4. Create EC2 machine (Ubuntu)</h2>
<h2>5. Open EC2 and Install docker in EC2 Machine:</h2>
<button onclick="copyText()">#optinal

sudo apt-get update -y

sudo apt-get upgrade

#required

curl -fsSL https://get.docker.com -o get-docker.sh

sudo sh get-docker.sh

sudo usermod -aG docker ubuntu

newgrp docker</button>
<h2>6. Configure EC2 as self-hosted runner:</h2>
<button onclick="copyText()">setting>actions>runner>new self hosted runner> choose os> then run command one by one</button>
<h2>7. Setup github secrets:</h2>
<button onclick="copyText()">AWS_ACCESS_KEY_ID=

AWS_SECRET_ACCESS_KEY=

AWS_REGION = us-east-1

AWS_ECR_LOGIN_URI = demo>>  566373416292.dkr.ecr.ap-south-1.amazonaws.com

ECR_REPOSITORY_NAME = simple-app</button>