[![CI](https://github.com/rubyonracetracks/docker-debian-install/actions/workflows/ci.yml/badge.svg)](https://github.com/rubyonracetracks/docker-debian-install/actions/workflows/ci.yml)

# Installing Docker in Debian
This repository contains scripts for automatically installing Docker and other important development tools in an environment based on Debian Linux or one of its derivatives.

## Prerequisites
* You MUST be using an environment based on Debian Linux or one of its derivatives.
* If your host OS is Mac OS or Windows, you should install a Debian-based Linux virtual machine.  A procedure on how to do this is provided in the [VirtualBox Tutorial](https://www.virtualboxtutorial.com/).
* Git should be installed in your Debian installation.  If you have not installed Git, you can install it by entering the following command in the terminal:
```
sudo apt-get update; sudo apt-get -y install git
```

## Procedure
* Enter the following commands in the terminal:
```
cd
mkdir -p rubyonracetracks
cd rubyonracetracks
git clone https://github.com/rubyonracetracks/docker-debian-install.git
cd docker-debian-install
bash main.sh
```
* The last actions of the installation script include printing out the currently installed versions of Docker and Docker Compose and running the hello-world Docker image.  If all went well, these actions were successfully executed.
