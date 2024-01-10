#Clone the given repository to your local by using the code. 

#Run commands to Install Java
    #dnf update
    #yum install java-11-openjdk-devel

#Install Jenkins
    #https://pkg.jenkins.io/redhat-stable/
    #https://www.redhat.com/sysadmin/install-jenkins-rhel8

#you can enable the Jenkins service to start at boot with the command:
    #sudo systemctl enable jenkins

#You can start the Jenkins service with the command:
    #sudo systemctl start jenkins

#You can check the status of the Jenkins service using the command:
    #sudo systemctl status jenkins
    # systemctl status jenkins

#Change Inbound traffic rules in AWS edit traffic for ALL, This is only a personal project. In the company, we have to follow the provided steps.

#Run Private IP:8080 in a search engine to see it's working or not.

#Inside Jenkins install docker pipeline plugins form Manage Jenkins

#In Jenkins.

#Dashboard > Mange Jenkins > Plugins

#In plugins search for docker pipeline and sonar Qube scanner and Install it.

#Now install sonar server in AWS(Local)
    #adduser sonarqube

#and then change from root to  soanrqube
    #sudo su - sonarqube

#Use command to download binaries of sonarqube and then unzip it.
    #wget https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-9.4.0.54424.zip
    #unzip * 