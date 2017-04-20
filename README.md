### Sample Java-Tomcat helloworld app

![AyeAye](https://github.com/shippableSamples/node-build-push-docker-hub/blob/master/public/resources/images/captain.png)

# Sample Java/Tomcat app running in Docker container on Elastic Beanstalk
[![Run Status](https://api.shippable.com/projects/5885ecca11c45a1000af5760/badge?branch=master)](https://app.shippable.com/projects/5885ecca11c45a1000af5760)
[![Coverage Badge](https://api.shippable.com/projects/5885ecca11c45a1000af5760/coverageBadge?branch=master)](https://app.shippable.com/projects/5885ecca11c45a1000af5760)


A simple Java Hello World application with unit tests and coverage reports.

This repo demonstrates the following features:
* Set up serverless CI, i.e. on Shippable-provided infrastructure
* Set up CD pipelines for deploying a docker image to a Single Container Docker Configuration on Amazon Elastic Beanstalk
* Perform CI tests
* Perform Maven build to generate .war package
* Perform docker build to create Tomcat server with .war package
* Push docker image to Amazon ECR

## Run CI for this repo on Shippable
* Fork this repo into your source code account (e.g. GitHub)
* Create an account (or login) on [Shippable](www.shippable.com) with your SCM account
* Create an [integration](http://docs.shippable.com/integrations/imageRegistries/ecr/) 
on Shippable for authenticating CI to AWS
* Update the CI configuration in `shippable.yml` file with your integration names 
(see comments in file)

### CI console screenshot
![CI Console Log](https://github.com/shippableSamples/java-ecr-runcli-elasticbeanstalk/blob/master/resources/images/java-ecr-runcli-elasticbeanstalk-CI.png)


