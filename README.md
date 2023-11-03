Hello World! (WAR-style)
===============

This is the simplest possible Java web application which contains hello world.  



INSTALLATION AND SETUP
======================

STEP-1
-----------
create a ec2 instance

STEP-2
------------
install jenkins and tomcat in same instance with portno 9090 and 8080  respectively.

STEP-3
----------
create a pipeline-job and write a pipeline which create a war file and deploy the application in tomcat-server directly.

STEP-4
-----------
setup webhook from git providing jenkins url 

STEP-4
----------
select pipeline script from scm and provide the git url which contain Jenkinfile and provide the git credentials

STEP-5
----------
install some plugins such as Deploy to conatiner and

STEP-6
----------
provide the credentials of tomcat server in jenkins so that tomcat will integrate with jenkins

STEP-7
-------
after all the configuration build the job and check weather the job is build is sucess or fail.


-x-x-x--x-x-x-x-x--x-x-x-x-x-x-x

DIFFICULT PART
--------------------
1. to set up monitoring and grafana tool for the application 


-x-x--x-x-x-x-x---x-x-x-x-
GIT URL

https://github.com/Rohannegi11/hello-world-war.git
