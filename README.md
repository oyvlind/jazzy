# ROS2 jazzy jalisco Docker container
Built on docker.io/osrf/ros using osrf/jazzy-desktop-full

## 1. Pull OSRF docker image
Pre-requisits:
VS-code with GitHub and Docker extensions

In your VS code terminal, run: 
'docker pull osrf/ros:jazzy-desktop-full'

Verify with:
'docker run hello-world'

Clone this github repo to a suitable directory.

Run docker the OSRF ROS2 image

Build Docker container on the now running image. 

## 2 User configuration files
In workspace directory add folder *.config*, containing *user_config* (no file extention)
**user_config file should contain the follwoing:** 
`USERNAME=<"your-host-computers-username"> // use ${whoami} in terminal if you are unsure.
GIT_USER_NAME=<"github username">
GIT_USER_EMAIL=<"github user email">
WORKSPACE_PATH=<"local path to workspace directory>"`

*The userconfig files are launched from the **devcontainer.json** "postCreateCommand"*

## Network-setup
