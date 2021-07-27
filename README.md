
To run it via docker-compose 

# sonarqube-docker

sysctl -w vm.max_map_count=262144

docker-compose up -d

Once it's done, you can go to localhost:9000 or the <hostname>:9000 if you are using any other servers.
  
  
  ###########################################################################
  
  To run it via Dockerfile, please go to the folder where Dockerfile, run.sh and sonar.sh is present
  
  #1. docker build -t sonarqube-test .
  
  #2. docker run -d --name sonarqube.est -e SONAR_ES_BOOTSTRAP_CHECKS_DISABLE=true -p 9000:9000 sonarqube-test:latest
  
  #3. Go to http://<IP>:9000
  
  #4. The default user and password is admin/admin. It will prompt you to change the password once the UI is up.
  
  Good luck on seting up th SonarQube environment.
  
