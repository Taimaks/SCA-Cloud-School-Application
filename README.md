# SCA-Cloud-School-Application
Jenkins pipeline syntax used for Jenkinsfile.
=============================================
Syntax
------
pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Taiwo is getting into SCA-Cloud-School-Application.'
            }
        }
    }
}

It is a very simple pipeline which is only doing one step for build.
And it is prompting with the "Taiwo is getting into SCA-Cloud-School-Application."

Key Steps:
==========
To download and install Jenkins:
---------------------------------

To ensure that your software packages are up to date on your instance, use the following command to perform a quick software update:

[ec2-user ~]$ sudo yum update –y
Add the Jenkins repo using the following command:

[ec2-user ~]$ sudo wget -O /etc/yum.repos.d/jenkins.repo \
    https://pkg.jenkins.io/redhat-stable/jenkins.repo
Import a key file from Jenkins-CI to enable installation from the package:

[ec2-user ~]$ sudo rpm --import https://pkg.jenkins.io/redhat-stable/jenkins.io.key
[ec2-user ~]$ sudo yum upgrade

Install Java:
-------------
[ec2-user ~]$ sudo amazon-linux-extras install java-openjdk11 -y
Install Jenkins:

[ec2-user ~]$ sudo yum install jenkins -y
Enable the Jenkins service to start at boot:

[ec2-user ~]$ sudo systemctl enable jenkins
Start Jenkins as a service:

[ec2-user ~]$ sudo systemctl start jenkins
You can check the status of the Jenkins service using the command:

[ec2-user ~]$ sudo systemctl status jenkins

Connect to Jenkins
-------------------
Open Jenkins on web browser with your instance IP with port 8080

Instance ip with port for Jenkins:
----------------------------------
3.95.63.63:8080
