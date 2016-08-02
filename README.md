# Jenkins

This repository contains steps to setup jenkins on ubuntu server and creating jenkins job to run **selenium webdriver** and **appium** tests.

```
wget -q -O - https://jenkins-ci.org/debian/jenkins-ci.org.key | sudo apt-key add -
sudo sh -c 'echo deb http://pkg.jenkins-ci.org/debian-stable binary/ > /etc/apt/sources.list.d/jenkins.list'
sudo apt-get update
sudo apt-get install jenkins

sudo apt-get update
sudo apt-get install jenkins

```

###OR###
download war file from here https://updates.jenkins-ci.org/download/war/

and run 
```java -jar jenkins.war```


### Android Emulator setup###

- create emulator
- get list of available anddroid targets and abis
''' android list targets ```
- create emulator with latest android target
''' android create avd -n test -t android-24 --sdcard 512M --abi default/x64 '''
- start emulator 
``` emulator avd test --no-window --no-skin ```


