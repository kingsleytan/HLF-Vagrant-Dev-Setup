# Part of the course on Hyperledger Fabric
http://www.ACloudFan.com
https://hyperledger.github.io/composer/installing/installing-prereqs#ubuntu

Vagrant commands
================
> vagrant up
> vagrant ssh
> vagrant halt
> vagrant destroy

Windows | Mac | Linux Docker
============================
+ DO NOT RUN DOCKER DAEMON on Host Machine
+ Install the Docker or Docker toolbox - Only docker client will be used
+ Make sure that following environment variables are NOT SET
  Use Control Panel on windows
  DOCKER_TLS
  DOCKER_TLS_VERIFY
+ Set the Environment following variable in Windows 
  DOCKER_HOST=tcp://localhost:2376

Setup Vagrant Dev Environment
=============================
> Open a terminal window and cd to the root of this project
> vagrant up
> vagrant ssh
  $ ./scripts/install-prereqs.sh
// Logout of vagrant
  $ logout
> vagrant ssh
  $ ./scripts/install-composer.sh
  $ ./scripts/install-fabric-tools.sh

Validation
==========
You should be able to use the *docker* commands on your host machine
> set DOCKER_HOST=tcp://localhost:2376
> docker ps     // Should not fail