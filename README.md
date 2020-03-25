# recipe-app-api
Recipe app api source code

- DockerFile Image : we are using python 3.7-alpin image [Link](https://github.com/docker-library/python/blob/695bd3c10cdf1692a2af9abdc51f0eff99731e78/3.7/alpine3.11/Dockerfile)
- [Dockerfile](https://gist.github.com/LondonAppDev/27c64d2c2df3555470812d4d77611389)
- requirement.txt : contains all the requirements 
- Docker Compose : This allow us to run docker images

``docker build .`` [Doc Link](https://docs.docker.com/engine/reference/builder/) 

``docker-compose build`` // this will build our image using docker-compose config

``docker-compose run service_name sh -c "django-admin.py startproject app ."
 i.e docker-compose run app sh -c "django-admin.py startproject app ."``  // creating Django project using a docker configuration
 
 - [Travis](https://travis-ci.org/) : Tool for continuous integration  that let us automate some of the tests and checks on our project every time 
 we push it to github.
 
 - Travis CI config file is the file that tells travis what to do every time we push the change to our project.