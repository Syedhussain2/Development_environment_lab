# Development Environment Lab

## Introduction
This readme is a guide to setup  a virtual machine, using step guidance and commands. 
## Requirements
You will need vagrant and virtual Box.

### Steps to Download

### Setting up Vagrant

Step 1: Is to create a Vagrantfile. The purpose of the Vagrantfile is to mark the root directory of your project. Many of the configuration options are relative to this root directory. It also describe the kind of machine and resources you need to run your prokect, as wel as what softwares to install and how you want ot access it.

```
$ mkdir vagrant_getting_started
$ cd vagrant_getting_started
$ vagrant init

```
### Step 2: Call

``` 
Vagrant up

``` 
This creates the VM on the specifications given in the vagrant file.

### Step 3: Access VM

```
vagrant ssh

```

#### Step 4: Update and Upgrade

```
sudo apt-get  update && upgrade

```

### Step 5: Install Server

```
Install web-server nginx

```

### Step 6: Connecting to the Server

Check if the server is running , enter the following command:

```
curl http://localhost

```
Followed by : 

```
ifconfig

```
Editing ip address, go onto the vagrantfile and manually input this command in order to change the ip address. 

```
config.vm.network "private_network",  
ip:"192.168.10.100"
config.hostsupdater.aliases = ["development.local"]

```
