# Guia de Instalação Jenkins Centos 7

### 01 - Instalando java 

```
 sudo yum install -y java-1.8.0-openjdk-devel 
```

### 02 - Configurando repositório

```
sudo yum install -y wget

sudo wget -O /etc/yum.repos.d/jenkins.repo https://pkg.jenkins.io/redhat/jenkins.repo

sudo rpm --import https://pkg.jenkins.io/redhat/jenkins.io.key
```

### 05 - Instalando jenkins

```
sudo yum install -y jenkins

#Senha de desbloquio do Jenkins
cat /var/lib/jenkins/secrets/initialAdminPassword


#gerando senha segura no shell

date +%s | sha256sum | base64 | head -c 32 ; echo


```
