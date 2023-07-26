# PROJECT 5: Continues Integration using Jenkins, Sonarqube, Nexus and Slack

In this project, I deployed a continues integration for project #4 with Jenkins, Used Sonarqube to analyse the code for bugs, configured Nexus to Store artifacts, and slack to send notifications on build status. All these services were deployed on three EC2 instances Running Ubuntu and Linux Os. This project was much fun, Jenkins was configured to launch a build job each time a new commit was detected in Github repo(configured through Webhooks). The Jenkins, using the installed plugins runs code build with Maven, code analysis with Sonarqube(which analysis for bugs) if the threshold is acceptable for the set values, the code is stored in Nexus artifact repository where versionning is enabled with timestamp and build number. 

## Project Architecture and Dataflow
### Architecture
![Project Architecture](https://github.com/Ndzenyuy/CI-with-jenkins/blob/main/images/Project5_architecture.jpg)
### Dataflow
![Project dataflow](https://github.com/Ndzenyuy/CI-with-jenkins/blob/main/images/CICD%20data%20flowchart.jpg)

## Services 
- AWS EC2 instances
- Jenkins
- Sonarqube
- Nexus Artifact Repository
- Slack Bot-App for Jenkins CI

## Results
### Triggered Builds in jenkins
![build with jenkins](https://github.com/Ndzenyuy/CI-with-jenkins/blob/main/images/Screenshot%20from%202023-07-26%2011-24-55.png)
### Successful builds notification on slack
![success notifications on slack](https://github.com/Ndzenyuy/CI-with-jenkins/blob/main/images/Screenshot%20from%202023-07-26%2011-26-15.png)
### Nexus repository on Nexus server
![nexus repo](https://github.com/Ndzenyuy/CI-with-jenkins/blob/main/images/Screenshot%20from%202023-07-26%2011-42-11.png)
### Archived Artifacts
![archived artifacts](https://github.com/Ndzenyuy/CI-with-jenkins/blob/main/images/Screenshot%20from%202023-07-26%2011-42-56.png)
### Quality gate pass
![quality gate pass](https://github.com/Ndzenyuy/CI-with-jenkins/blob/main/images/Screenshot%20from%202023-07-26%2013-08-18.png)
