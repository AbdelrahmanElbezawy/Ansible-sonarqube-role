Role Name
=========

Ansible role to deploy sonarqube serive on ubuntu



problem
========
There is an issue that ansible can not login posgresSQL (work in ubuntu VMware)
maybe the problem that user's passwords
I do it manually by ssh to do this
#su - postgres
#createuser sonar
#psql
#ALTER USER sonar WITH ENCRYPTED password 'sonar';
#CREATE DATABASE sonarqube OWNER sonar;
#grant all privileges on DATABASE sonarqube to sonar;
#\q
