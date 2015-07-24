# openstackwurtzite-base

This is the openstackwurtzite base container, this base container is used to create all other containers. The contaneris based on the CentOS 7 image.

##Helper scripts
This repo has a number of helper scripts,

build-container: This script will run the command to build the container and give the contaner the correct image name.

push-contaner: This script will push the already built container to docker hub so that other may use it as a base to built further containers. You will need to be loged into docker hub before you run this command. As we are pushing the base container to one openstackwurtzite community repo you will need to login using the openstackwurtzite login or ask one of the members with admin to push it for you. This process will change in the future.

Directory & Files

/etc/wurtzite/metadata.json is used to hold the metadata about the container. The container agent will present this info through it API to the container manager. This file is normally created at buiild time an populated with the required info such as version, build date, dependacys, etc. The file is injected to the container buing the build. To get access to the info in this file you cna call the container agent API and this will return the entire json file for parshing. The container manager will use the metadata to better understand the requirements for the container and how it should handle the contaner.

TODO: Create a section on the layout of this file and how each parameter works and what it dose and how it shoul be used.
