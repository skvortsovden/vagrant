# Vagrant

The storage for [Vagrant](https://www.vagrantup.com/) configuration files

## What is Vagrant?

Vagrant is a tool for building and managing virtual machine environments in a single workflow. 

source: https://www.vagrantup.com/intro/index

## Vagrant Getting Started

### Create VM

```cmd
mkdir new-vm
cd new-vm
vagrant init hashicorp/bionic64
```

Where `vagrant init` - initializes the current directory to be a Vagrant environment by creating an initial Vagrantfile if one does not already exist.

**hashicorp/bionic64** - Ubuntu 18.04.6 LTS (Bionic Beaver)

### Start VM

Run command within the `new-vm` directory

```
vagrant up
```

### Login to VM

```
vagrant ssh
```
equals
```
ssh -p <port> vagrant@localhost
```

Where **port** can be found by `vagrant port` command and the password is **vagrant**.