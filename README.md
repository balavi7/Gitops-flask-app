***Jenkins and ArgoCD GitOps Demo for Kubernetes Deployment***
The CI part is managed by Jenkins, while the CD part is handled by ArgoCD using the GitOps approach.

Jenkins Installation
Jenkins is installed on an EC2 instance. Please follow the instructions provided in the link for installation. Note that you can skip the "Configure a Cloud" part for this demo. Be aware that some commands may yield errors; refer to the following workarounds:

If you encounter a daemonize error during the command sudo yum install jenkins java-1.8.0-openjdk-devel -y, follow the solutions provided in this Stack Overflow thread.

After Jenkins installation, install Docker on the EC2 instance by following the instructions outlined here.

Run sudo chmod 666 /var/run/docker.sock on the EC2 instance after Docker is installed.

Install Git on the EC2 instance by running sudo yum install git.

Jenkins Plugins
Install the following Jenkins plugins for the demo:

Amazon EC2 plugin (No need to set up Configure Cloud afterward)
Docker plugin
Docker Pipeline
GitHub Integration Plugin
Parameterized trigger Plugin
ArgoCD Installation
Install ArgoCD in your Kubernetes cluster by following the provided link.

Happy deploying!





