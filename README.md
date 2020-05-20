## Jenkins for Raspberry Pi (ARM 64, aka aarch64) 

Jenkins image for Docker on Raspberry Pi. 
(Tested on Raspberry Pi 3 (arm 64))

## build image
docker build --tag jenkins-arm64:1.0 .

## run image
docker run -d -p 8080:8080 -v $PWD/jenkins:/var/jenkins_home:z -t jenkins-arm64:1.0
