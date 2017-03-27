# Running GitLab CE in a Vagrant Centos7 VM

*Used on Mac OS X Sierra 10.12.3*

## Software Platforms version
1. Vagrant version 1.9.1
2. Virtual Box version 5.1.12


## Install Virtual Box Guest Additions plugin

The official Centos7 Vagrant Box does not come with virtualbox Guest Addtions installed.

There is a Vagrant Plugin however which will automatically do this for you.
Run command:
```
vagrant plugin install vagrant-vbguest
```


## Commands to run

```
vagrant up 

```

This installs and configures Gitlab as recommeded by GitLab instructions shown on this page:
https://about.gitlab.com/downloads/#centos7

Once installed an configured, you need to find the external IP for you Vagrant VM and go to the GitLab Login Page in a browser.

http://<your vm ip>/

Note that by default only an HTTP interface is enabled.

At the Login page you will be asked for the root account password you would like to set.
