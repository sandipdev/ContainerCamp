# Container Camp #
The official un-official container camp used to build out containerized applications on Azure.

> We assume you have an Azure Subscription...

## Azure Setup:  ##
This will setup cmd line access to Azure and works on OSX, Linux, even Windows.... At the bottom of setup step one, there is a Docker Image that will run the CLI in a container. Don't you think that's the right choice for this...

* Setup Step One 	- [Install Azure CLI](setup/xplat-cli-install.md)
* Setup Step Two 	- [Login to Azure CLI](setup/xplat-cli-login.md)
* Setup Step Three 	- [Switch Azure CLI to ARM Mode](setup/xplat-cli-arm.md)
* Setup Step Four	- [Install Docker for Windows](https://www.docker.com/)

## Lab One: Getting Familiar with Azure Resource Manager ##
This lab will get you familiar with using the Azure CLI for deploying resources to Azure. We'll use Azure Resource Manager (ARM) Templates to describe what we want created in Azure. For More information about ARM and ARM Templates see: [Azure Resource Manager Overview](labone/arm-overview.md).

* [Deploy a simple Linux VM using the Quick Start Templates and the Azure CLI](labone/deploy-simple-linux.md)

## Lab Two: Run Docker on a VM in Azure ##
In this lab you will setup a VM like in labone, but it will have docker... We'll deploy nginx and hit the default website from a browser.

* [Deploy a Docker VM using the Quick Start Template](labtwo/deploy-docker-vm.md)

## Lab Three: Configure a Windows Container Host ##
In this lab you will build a Windows 2016 Server TP5 Container Host and deploy Windows containers.

* [Windows Containers on Windows Server](labthree/windows-containers.md)

## Lab Four: Setup Docker Swarm and Deploy Some Containers ##
In this lab you will deploy Docker Swarm. Once you have a swarm you will deploy some things to it...

* [Deploy Docker Swarm](labfour/deploy-docker-swarm.md)

> **NOTE** -- In this lab we need to switch azure-cli mode from ARM to ASM. We'll also be using a secure docker endopoint see [Protect the Docker daemon socket](https://docs.docker.com/engine/security/https/) for more information.

## Lab Five: Setup Azure Container Service ##
In this lab we'll look at Microsoft Azure's Container as a Service solution called: Azure Container Service (ACS).

* [Deploy Azure Container Service](labfive/deploy-acs.md)
* [Connect and Use ACS](labfive/connect-acs.md)