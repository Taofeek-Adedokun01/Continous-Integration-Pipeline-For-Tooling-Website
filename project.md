## Step 1 – Install Jenkins server

## Create an AWS EC2 server based on Ubuntu Server 20.04 LTS and name it "Jenkins"

`sudo apt update`

`sudo apt install default-jdk-headless`

`wget -q -O - https://pkg.jenkins.io/debian-stable/jenkins.io.key | sudo apt-key add -
sudo sh -c 'echo deb https://pkg.jenkins.io/debian-stable binary/ > \
    /etc/apt/sources.list.d/jenkins.list'`

`sudo apt update`

`sudo apt-get install jenkins`

`sudo systemctl status jenkins`

![Jenkins-status](./images/Jenkins-status.PNG)

![Jenkins:8080](./images/Jenkins-8080.PNG)

## Step 2 – Configure Jenkins to retrieve source codes from GitHub using Webhooks

![Last-Build](./images/Last-build.PNG)
## Step 3 – Configure Jenkins to copy files to NFS server via SSH

![Jenkins](./images/jenkins.PNG)

![Changes-on-webhook](./images/Changes-on-webhook.PNG)

![Test-configuration](./images/testconfiguration.PNG)

![Console-output](./images/Console-output.PNG)

![NFS](./images/NFS.PNG)

