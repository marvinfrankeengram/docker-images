# Jenkins-Slave

Basically a full-blown dev machine, allowing you to

- Build a java8 backend
- Containerize it using docker
- Push Image to ECR
- Build a js-Frontend (you still need to provide node though)
- Test frontend via puppeteer
- Package frontend as electron app

This one-stop-shop approach comes at a prize though: the image clocks in a hefty
5gb size.

Inspired by evarga/docker-images and mzagar/jenkins-slave-jdk-maven-git

- FROM ubuntu:disco
- git
- Open JDK 8
- python3 & pip
- aws-cli
- ECR credentials helper
- jq
- Maven 3.6.3
- Jenkins user
- SSH access
- Various libraries needed to run chrome via puppeteer
- docker
- Build-Essentials
- (un)zip
- wine
