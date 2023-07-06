[![CI](https://github.com/rubyonracetracks/docker-debian-install/actions/workflows/ci.yml/badge.svg)](https://github.com/rubyonracetracks/docker-debian-install/actions/workflows/ci.yml)

# Installing Docker in Debian
This repository contains scripts for automatically installing Docker in an environment based on Debian Linux or one of its derivatives.

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
* The installation of Docker will take a few minutes.  The last steps will include running the hello-world Docker image (to confirm that Docker works) and printing the versions of Docker and Docker Compose that were installed.
* Open the file manager.  Go to the rubyonracetracks directory you created in your user home directory.  Delete the docker-debian-install directory, because you no longer need it.
