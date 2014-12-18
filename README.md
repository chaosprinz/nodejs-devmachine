# NodeJs-Devmachine

This is a basic development-environment in a Vagrant-box, built by using Chef.
I use Ubuntu 14.04-Trusty Thar as the base. Chef is used to install necessary
packages and setting things up.

## Configuration

Configuration is done through the vm.conf.yml-file. At the moment the following
options can be set in this file:
- box: A string, telling vagrant the base-box to use. Required
- ip: A string, setting the static ip. Required
- forwards: An array of hashes. Each hash needs two elements: guest and host.
Each describes a port, given as string. Optional
