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
```
* To install Docker and other important development software, enter the command ```bash main.sh```.  This will take a few minutes.
* If you just want to install Docker and skip installing the other software, enter the command ```bash install-docker-only.sh```.
* When the script is finished, reboot your Debian-based Linux installation.
* Open the file manager.  Go to the rubyonracetracks directory you created in your user home directory.  Delete the docker-debian-install directory, because you no longer need it.
* Enter the following command in the terminal:
```
docker --version
```
* You should now see the Docker version installed, and there should be NO error message.
* Congratulations!  You have successfully installed Docker.
