This is a script that will install ELK stack 7.x on your system.

Great for users who want to install quickly or for those who are new to ELK and want to get up and running with less confusion.  Searching on the web and even using the installation guides on [elastic's website](https://www.elastic.co) can be confusing.  ELKscript will cut out most of the installation frustration.

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