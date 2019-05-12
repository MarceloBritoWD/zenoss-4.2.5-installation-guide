# Instalation guide of Zenoss 4.2.5 on CentOS 5/6

## Steps bellow:

- First, install the CentOs 6 ISO (http://isoredirect.centos.org/centos/6/isos/i386/) on your machine (make sure to have at least 4GB free on the file system);
- Then, as root user, you will need to remove some packages using yum package control (it will be installed by the autodeploy script);
  - yum remove mysql* or yum remove MySQL*
  - yum remove java*
- Then, download and install the JRE 8 (https://www.oracle.com/technetwork/pt/java/javase/downloads/jre8-downloads-2133155.html)
- Now you can follow the official auto-deploy documentation (http://wiki.zenoss.org/Install_Zenoss#Auto-deploy_Installation);
  
  ATTENTION: Don't run the ./core-autodeploy.sh file, it has some problems that I solved on the file with the same name on this repository, download it and run.
 
- At the end (it can take a few minutes), If Everything works well, Zenoss 4.2.5 will be running on localhost:8080
