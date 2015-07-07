# openstackwurtzite-baseimage

This is the openstackwurtzite base image, this base image is used to create all containers. This base image is created from a CentOS 7 image.

##Helper scripts
This repo has a number of hemper scripts,

build-container: This script will run the command to build the container and give it the correct name.

push-contaner: This script will psh the already built container to the docker hub so that other may use it as a base to built further containers. You will need to be loged into docker hub before you run this command. As we are pushing the base container to one openstackwurtzite community repo you will need to login using the openstackwurtzite login or ask one of the members with admin to push it for you. This process will change in the future.

