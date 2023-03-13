This script is a Bash script for installing Elasticsearch, Kibana, and Logstash on a Debian-based Linux system. It first updates and upgrades the system packages, installs necessary dependencies such as apt-transport-https, ca-certificates, and gnupg2, and adds the Elasticsearch repository to the sources list.

After that, the script installs Elasticsearch, starts the Elasticsearch service, and checks the status of Elasticsearch using curl. Next, it installs Kibana, starts the Kibana service, and finally installs and starts Logstash.

The script uses various commands such as apt-get, wget, systemctl, and curl to install and manage the services. It also uses color codes to make the output more readable and informative. Overall, the script automates the installation process for Elasticsearch, Kibana, and Logstash, saving you time and effort.

Searching on the web and even using the installation guides on [elastic's website](https://www.elastic.co) can be confusing.  ELKscript will cut out most of the installation frustration.

## Prerequisites

- System must be Debian-based / Ubuntu.  Not ARM architecture
- Other OS flavors like RedHat, Centos, OpenSuSE require rpms and those are not supported with this script
- Recommend you have a static IP set for your system.
- Must be able to elevate to root

## How To Use

1. Copy, then navigate to ELKscript in the system where you want to run the ELK stack 

```
git clone https://github.com/belalelmi/The-ELK-Installation-Script-.git && cd ELKscript

```

2. Make ELKscript executable 

```
sudo chmod +x ELKscript
```

3. Run ELKscript

```
sudo ./ELKscript
```

ELKscript will perform the following steps:

1. System Update
2. Install Java 8 as required to run ELK
3. Install Elasticsearch 7.x
4. Install Kibana 7.x
5. Install Logstash 7.x
6. Set Elasticsearch, Kibana, and Logstash to start on boot
7. Start all three services service 
