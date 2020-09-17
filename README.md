# DevOps2

With this will install 1 Ubuntu 18.04 machine. It will add some default users and groups.
This Vagrant is to practice the skills for adding users and groups and set permissions.
This repository is intended for educational purpose only.


## Prerequisites

Works on Windows 10 and tested on macOS (macOS needs the Virtualbox extension pack).

Software needed:
* Virtualbox 5.0 or higher
* Git bash for Windows
* Vagrant 2.2.6 or higher


## Demo installation && use Vagrant

Youtube: https://youtu.be/KABnIuaA8SM


## Installation

* Install Virtualbox: https://www.virtualbox.org/wiki/Downloads
* Install Git bash for Windows: https://gitforwindows.org/
* Install Vagrant for Windows: https://www.vagrantup.com/downloads.html

## Run this Vagrant VM
Open **Git Bash** in Windows
```
cd Documents
mkdir vagrant && cd vagrant
git clone https://github.com/borahuho/DevOps2
cd DevOps2
vagrant up
vagrant ssh
```
## Mission

Read your mission in ~/vagrant/mission

## Network
Vagrant VM will be set up with 2 network adapters
```
Nat : DHCP
Localhost : 192.168.10.5
```
## Vagrant commands
Make a new VM with Vagrant
```
vagrant up
```
Pause a VM
```
vagrant suspend
```
Restart a paused VM
```
vagrant resume
```
Stop and shutdown a VM
```
vagrant halt
```
Remove a VM
```
vagrant destroy
```
ssh in to the VM
```
vagrant ssh DevOps2
```

