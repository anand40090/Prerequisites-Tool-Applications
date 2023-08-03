# Prerequisites-Tool-Applications

### How to update Ubuntu 
```
sudo apt update -y
```

### How to install OpenJdk-11 DockerEngine Git Unzip 
```
sudo apt install openjdk-11-jdk docker.io git unzip -y
```

### How to install [Jenkins](https://phoenixnap.com/kb/install-jenkins-ubuntu)

```
1. Step 1: Install Java >> sudo apt install openjdk-11-jdk
```
```
2. Step 2: Add Jenkins Repository

curl -fsSL https://pkg.jenkins.io/debian/jenkins.io-2023.key | sudo tee \
  /usr/share/keyrings/jenkins-keyring.asc > /dev/null

echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] \
  https://pkg.jenkins.io/debian binary/ | sudo tee \
  /etc/apt/sources.list.d/jenkins.list > /dev/null
```
```
3. Step 3: Install Jenkins

sudo apt update

sudo apt install jenkins -y

sudo systemctl status jenkins

sudo systemctl enable --now jenkins

```
```
4. Step 4: Modify Firewall to Allow Jenkins

1. Open port 8080 by running the following commands: sudo ufw allow 8080 && sudo ufw status

2.  If you haven't configured the UFW firewall yet, it displays as inactive : sudo ufw enable
```
```
5. Step 5: Set up Jenkins

1. Open a web browser, and navigate to your server' IP address. Use the following syntax: http://ip_address_or_domain:8080

2. Obtain the default Jenkins unlock password by opening the terminal and running the following command:
sudo cat /var/lib/jenkins/secrets/initialAdminPassword

3. The system returns an alphanumeric code. Enter that code in the Administrator password field and click Continue.

4. The setup prompts to either Install suggested plugins or Select plugins to install. It’s fine to simply install the suggested plugins.
```

### How to install [sonqrqube & PostgreSQL](https://linux.how2shout.com/install-sonarqube-on-ubuntu-20-04-18-04-server/)

1. Run Ubuntu system update
2. Install Java OpenJDK
3. Create a Dedicated user for Sonarqube
3. Install PostgreSQL Database [Option1](https://ubuntu.com/server/docs/databases-postgresql) [Option2](https://www.postgresql.org/download/linux/ubuntu/) [Option3](https://www.cherryservers.com/blog/how-to-install-and-setup-postgresql-server-on-ubuntu-20-04)
4. Create a database for Sonar
5. Download and Setup SonarQube on Ubuntu 20.04/18.04
Configure Database for Sonar
6. Create a SonarQube Systemd service file
7. Allow Sonarqube port in Ubuntu 20.04 firewall
8. Access the Sonarqube Web interface

### How to install [Jfrog](https://computingforgeeks.com/how-to-install-jfrog-artifactory-on-ubuntu/?expand_article=1)

### How to install [Apache Maven](https://www.digitalocean.com/community/tutorials/install-maven-linux-ubuntu) /  [Download Maven](https://maven.apache.org/download.cgi)
