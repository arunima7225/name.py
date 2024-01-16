JENKINS DOWNLOAD AND DEPLOYMENT

Ref: https://pkg.jenkins.io/debian-stable/


  sudo wget -O /usr/share/keyrings/jenkins-keyring.asc \
    https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key

     echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] \
    https://pkg.jenkins.io/debian-stable binary/ | sudo tee \
    /etc/apt/sources.list.d/jenkins.list > /dev/null

      sudo apt-get update
  sudo apt-get install fontconfig openjdk-17-jre
  sudo apt-get install jenkins


chmod 400 "jenkins_arunima.pem"
ssh -i "jenkins_arunima.pem" ubuntu@16.170.230.28


 cd  /var/lib/jenkins/workspace
