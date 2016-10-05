Provisioning a new site
=======================

## Required Packages

* nginx
* Python 3
* Git
* pip
* virtualenv

eg, on CentOS 6:

    sudo yum install nginx git python3 python3-pip
    sudo pip3 install virtualenv

## Nginx Virtual Host Config

* see nginx.template.conf
* replace SITENAME with, eg, shijun.wang

## Upstart Job

* see gunicorn-upstart.template.conf
* replace SITENAME with, eg, shijun.wang

## Folder Structure
Assume we have a user account at /home/username

    /home/username
    └── sites
        └── SITENAME
            ├── database
            ├── source
            ├── static
            └── virtualenv
