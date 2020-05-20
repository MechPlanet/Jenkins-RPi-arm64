## Jenkins Raspberry Pi image for ARM64 

Jenkins for Docker on Raspberry Pi

## build image
docker build --tag jenkins-arm64:1.0 .

## run image
docker run -d -p 8080:8080 -v $PWD/jenkins:/var/jenkins_home:z -t jenkins-arm64:1.0
