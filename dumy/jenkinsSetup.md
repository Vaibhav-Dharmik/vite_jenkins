<!-- Command to set path to work with docker jenkins -->

docker stop jenkins
docker rm jenkins
docker run -d -p 8080:8080 -p 50000:50000 ^
-v jenkins_home:/var/jenkins_home ^
-v "C:/Users/Vaibhav_Dharmik/Desktop/NeoUtilix Projects practise/jenkins-test":/var/jenkins_home/workspace/jenkins-test ^
--name jenkins jenkins/jenkins:lts
