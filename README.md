# ROS2 jazzy jalisco Docker container
Built on docker.io/osrf/ros using osrf/jazzy-desktop-full

## 1. Pull OSRF docker image
Pre-requisits:  
   VS-code with GitHub and Docker extensions

In your VS code terminal, run:  
    `docker pull osrf/ros:jazzy-desktop-full`

Verify with:  
    `docker run hello-world`

Clone this github repo to a suitable directory.  
Run docker the OSRF ROS2 image  
Build Docker container on the now running image. 

## 2 User configuration files
In workspace directory add folder *.config*, containing *user_config* (no file extention)  
**user_config file should contain the follwoing:**   
`USERNAME=<"your-host-computers-username"> `  use  `${whoami} in terminal if you are unsure of username format.`  
`GIT_USER_NAME=<"github username">`    example username format: `"opensourceror"`  
`GIT_USER_EMAIL=<"github user email">` example:`"opensourceror@closed.com"`  
`WORKSPACE_PATH=<"local path to workspace directory>"` example `"/home/sourceror/jazzy_workspace"`  

*At the moment the userconfig files are launched from the **devcontainer.json** "postCreateCommand"*
Not fully functioning yet, so please search for capital letters: **REPLACE**, to find elements you need to replace with your own.

## Network-setup
Soon to come.
