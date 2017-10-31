Tweet app revisited to build, test, deploy using an automated CI-CD pipeline with Wercker deployed as containers on AWS.

[![wercker status](https://app.wercker.com/status/9cac93950da19c6b6ae466fc53458cd0/s/master "wercker status")](https://app.wercker.com/project/byKey/9cac93950da19c6b6ae466fc53458cd0)  [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/dwyl/esta/issues)



Introduction

This post is to help you set up a CI-CD pipeline using wercker for the application running on docker container. Same can be used to scale out or for bigger applications as well. It would serve as a initial starting point to set up pipeline and workflows on wercker. 
This would also help you with Slack integration step to post notifications on your build status. 

Documentations

<a href="http://devcenter.wercker.com/docs/home">Learn about wercker</a>

<a href="https://www.docker.com/sites/default/files/Docker_CheatSheet_08.09.2016_0.pdf">Docker Commands/Cheat Sheet</a>

Pre-requisites 

Dockerhub Account to store your docker images - <a href="https://hub.docker.com/">create your free docker hub account</a>

Wercker Account for your CI-CD pipeline - <a href="http://www.wercker.com/pricing">create your free wercker account</a>

A running EC2 Instance. ( Note: <a href="https://docs.docker.com/engine/installation/#prior-releases">Install docker on the EC2 Server</a> )

Application

<a href="https://github.com/dockersamples/linux_tweet_app">Source Code of the Application's HTML file</a>

Wercker:

1. Integrating werkcer with git. 
On the profile page, open up setting and git connections underneath settings. You would have option to either connect to your github account or bitbucket account.

2. Creating the application. 
