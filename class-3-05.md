# Heroku

## Introduction

Heroku is a program and service that allows you to deploy a web project, or app, along with the server, to a public account so that you can allow your client to see the product, yet prevent the entire public from seeing it. It works with Node and consequently with npm. 

One of it's key advantages is being easily streamlined with Github, allowing for easy and synchronized updates. It also allows you to run a local test site or dev site without using live server. This is helpful since it allows the developer to control the server in a way that before he could not. 

## Procfile

What is a procfile? A procfile is a textfile existing inside the root which declares explicitly every command to execute once the app is started. The example provided in the official documentation of how the procfile might do this is: 

`web: node index.js`

## Dyno

What is a dyno? The official Heroku documentation suggests that we consider a dyno as a 'lightweight container' which 'runs the command specified in the Procfile.'

Dynos may be free, and limited, or paid for with superior capabilities. The default dyno that is used is the free version, which will go to sleep if not being used, and has a monthly quota as well, which can limit it's use. Upgrades, naturally, take care of these problems. This is important to note, since if a developer runs out of hours, he will likely find his site not working upon refresh.

## Misc.

Heroku allows for all different kinds of add-ons. For example, some add-ons allow for better log tracking. You can also create a database, and you can use add-ons like MongoDB, Postgres and mySQL. In sum, Heroku is a cloud-based platform which provides service in many different programming languages, which, especially when connected to GitHub, makes deployment and project management simpler and quicker.