# jenkins-cli
Repository for Jenkins CLI 

## Project setup for Jenkins CLI

```
mkdir -p jenkins-cli/src/github.com/sriram-yeluri/jenkins-cli  
mkdir -p jenkins-cli/src/github.com/sriram-yeluri/jenkins-cli/glib  
mkdir -p jenkins-cli/src/github.com/sriram-yeluri/jenkins-cli/ds  
mkdir -p jenkins-cli/src/github.com/sriram-yeluri/jenkins-cli/jenkinslib  
mkdir -p jenkins-cli/pkg  
mkdir -p jenkins-cli/bin  
touch README.md  

export GOPATH=/home/sriram/goProjects/jenkins-cli/  
```
### Docker image of jenkins LTS is used to test this cli. 
[docker-hub-jenkins](https://hub.docker.com/r/jenkins/jenkins/)
pull jenkins images and spin a container. 

```
docker pull jenkins/jenkins
docker run -p 8080:8080 -p 50000:50000 jenkins/jenkins:lts
For persistance data, use local volume : 
docker run -p 8080:8080 -p 50000:50000 -v jenkins_home:/var/jenkins_home jenkins/jenkins:lts
```

For more details about managing jenkins image, click below link to visit official Jenkins git-hub page
[official-Jenkins-github](https://github.com/jenkinsci/docker/blob/master/README.md)
