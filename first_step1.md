#### Course Prerequisites: 
- Full Admin Access to your machine
- Installed JDK 1.8x
#### Acronyms: 
- SDLC - Software Development Lifecycle
- SCM - Software Configuration Management
- ELK - Elasticsearch, Logstash and Kibana
- GitFlow - Git Workflow
- SSH - Secure Shell
- Git - Version Control System
- CI - Continuous Integration
- Repository - Place to store the Artifacts
#### Required Tools:
- GitHub Account
- Install Git 
- Install Atlassian Source Tree: https://www.sourcetreeapp.com
- Optional: install Git Flow for Executing via command Line
- Download and install STS: https://spring.io/tools/sts/all
- Download Editor like ATOM and install: https://atom.io
- Download Maven: http://maven/apache.org
- Download Tomcat: https://tomcat.apache.org/download-80.cgi
- Download Artifactory: https://www.jfrog.com/open-source/
- Donwload Jenkins: https://jenkins.io/download
- Download ElasticSearch: https://www.elastic.co/downloads/elasticsearch
- Download Logstash: https://www.elastic.co/downloads/logstash
- Donwlaod Kibana: https://www.elastic.com/downloads/kibana
#### Install Of Tools:
1. Install Tomcat
    a. Install to Development
    b. Start Tomcat
    c. Validate setup
2. Install Artifactory
    a. Install to Development
    b. Start artifactory
3. Install Maven
    a. Install to development
    b. Setup Maven Home
    c. Validate Setup
4. Install Jenkins
    a. Install
    b. Start Jenkins
    c. Validate Setup
5. Install Elk 
    a. Install Elastic Search 
    b. Install Logstash
    c. Install Kibana
#### Install Apache Tomcat:
- Download all tools file in download folder.
- create a directory Devops, This will be using for other installtion too.
- Copy enitre tomcat directory from downlaod to Devops.
- Now make some configuration change for it.
    `vi tomcat-user.xml` (to create roles and user for tomcat)
    Create Two roles "manager-gui and manager-script" apart from the default.
    `chmod +x *.* ` (To make all files execute inside bin directory)
    `./cataline.sh start` (To start the tomcat, run this command from bin dir.)
    `tail ../logs/cataline.out` (To see the log)
- Now test tomcat using IP of the server.

#### Installation of Jfrog:
- use the url to install jfrog https://websiteforstudents.com/how-to-install-jfrog-artifactory-on-ubuntu-18-04-16-04/
### OR
- Download jfrog tar file from official site
- copy tar file in Devops folder
    `cp -R Download/artifactory Devops/`
- go to bin:
    `./artifactory.sh` ( To Run Artifactory )
- Test it to run http://Server_ip:8081 using default user (admin) and password (admin).
#### Installation of Jenkins:
- Use the url to install the jenkins: https://jenkins.io/download/ and choose appropriate OS to installation.
- Once installtion is completed, then use http://server_ip/8080 to do further configuration. 
- How to change Jenkins default port:
  `default read /Library/Preferences/org.jenkins-ci`
  `default write /Library/Preferences/org.jenkins-ci httpPort 8090`
  `sudo launchctl unload /Library/Preferences/org.jenkins-ci.plist`
  `sudo launchctl load /Library/Preferences/org.jenkins-ci.plist`

