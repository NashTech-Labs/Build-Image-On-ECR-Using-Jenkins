## Description
Here, In this template you will get to know about the steps of How to push an image of your application into the AWS ECR
repository using the Jenkins file.


### Steps:-
1. Login into the AWS account and spin up an instance of your compatibility like Ec2 micro or x2.large etc.
2. Configure it.
3. Install the Jenkins CI/CD tool and Docker.
4. Build your application for example , I have build my application on maven tool so I have used `mvn clean install` where it creates the `.jar` file which can be used to build the application image.
5. After building the application, logging into the Jenkins.
6. Push the changes in the github repository or any other repository where the source is written.
7. Configure the pipeline like adding the github repo and dependent plugins.
8. Trigger the pipeline.
9. Check into the ECR repository where the repo is created like I have created with the name `sample-demo` , here you will find your image.


### <u>Notes</u> 

* If you get any error related to docker permission denied in the pipeline use `sudo chmod 777 /var/run/docker.sock` .
