#Clone the given repository to your local by using the code.

#Run commands to Install Java
    <br>
    *dnf update
    <br>
    *yum install java-11-openjdk-devel

#Install Jenkins
    <br>
    #https://pkg.jenkins.io/redhat-stable/
    <br>
    #https://www.redhat.com/sysadmin/install-jenkins-rhel8

#you can enable the Jenkins service to start at boot with the command:
    <br>
    *sudo systemctl enable jenkins

#You can start the Jenkins service with the command:
    <br>
    *sudo systemctl start jenkins

#You can check the status of the Jenkins service using the command:
    <br>
    *sudo systemctl status jenkins
    <br>
    *systemctl status jenkins

#Change Inbound traffic rules in AWS edit traffic for ALL, This is only a personal project. In the company, we have to follow the provided steps.

#Run Private IP:8080 in a search engine to see it's working or not.

#Inside Jenkins install docker pipeline plugins form Manage Jenkins

#In Jenkins.
<br>
    *Dashboard > Mange Jenkins > Plugins

#In plugins search for docker pipeline and sonar Qube scanner and Install it.

#Now install sonar server in AWS(Local)
    <br>
    *adduser sonarqube

#and then change from root to  soanrqube
    <br>
    *sudo su - sonarqube

#Use command to download binaries of sonarqube and then unzip it.
    <br>
    *wget https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-9.4.0.54424.zip
    <br>
    *unzip *

#Will grant some permissions
    <br>
    #chmod -R 755 /home/sonarqube/sonarqube-9.4.0.54424
    <br>
    #chown -R sonarqube:sonarqube /home/sonarqube/sonarqube-9.4.0.54424
    <br>
    #cd sonarqube-9.4.0.54424/bin/linux-x86-64/
    <br>
    #./sonar.sh start

#*Sonarqube will start on the server port 9000

#Maven is connected with docker we have to connect sonarqube with jenkins
    <br>
    # sonarqube > my account > security > generate Token by the name Jenkins

#After genrating Token copy the code and then open jenkins
   <br>   #jenkins  >  Dashboard > Manage Jenkins > Crendentials > System > Global Credentials and then create crentials.

#To restart sonarqube
<br>
open server created by adduser sonarqube , then  ls and open the directory in that directory open bin and enter in linux folder then use start command .
<br>
#sudo su - sonarqube  >  ls >  cd ./sonarqube-9.4.0.54424 > cd ./bin > cd ./linux-x86-64 > ./sonar.sh start


#will install docker to the EC2 Instance
<br>
To remove existing containers 
sudo apt remove --purge docker docker-engine docker.io containerd runc

For CentOS:
<br>
sudo yum install -y yum-utils
<br>
sudo yum-config-manager --add-repo https://download.docker.com/linux/centos/docker-ce.repo
<br>
sudo yum install docker-ce docker-ce-cli containerd.io
<br>
sudo systemctl start docker
<br>
sudo systemctl enable docker

#whenever any kubernates controler is  used first install all the tools by using kuberbnates controllers. 
<br>
#How to install mikube. 
#https://phoenixnap.com/kb/install-minikube-on-centos

#Install kubernates operatore from operatorhub.io
For Example 
Argo CD > Install > Follow steps