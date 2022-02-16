Linux (Host/VM)
https://www.jenkins.io/doc/book/installing/linux/ 
1) wget -q -O - https://pkg.jenkins.io/debian-stable/jenkins.io.key | sudo apt-key add - 
2) sudo sh -c 'echo deb https://pkg.jenkins.io/debian-stable binary/ > \/etc/apt/sources.list.d/jenkins.list' 
3) sudo apt-get install jenkins 
 
● Docker https://hub.docker.com/r/jenkins/jenkins 
1) docker pull jenkins/jenkins 
2) docker run -p 8080:8080 -p 50000:50000 jenkins/jenkins:lts