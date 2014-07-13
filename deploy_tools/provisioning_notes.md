Provisioning a new site
=======================

## Required packages:

* nginx
* Python 3
* Git
* pip3
* virtualenv

eg, on Ubuntu:

	sudo apt-get install nginx git python3 python3-pip
	sudo pip3 install virtualenv

## Nginx Virtual Host config

* see nginx.template.conf
* replace SITENAME with, eg, staging.my-domain.com
* replace ubuntu with, eg, user-name 

## Upstart Job

* see gunicorn-upstart.template.conf
* replace SITENAME with, eg, staging.my-domain.com
* replace ubuntu with, eg, user-name

## Folder structure:
Assume we have a user account at /home/user-name

/home/user-name
+--sites
|  +--SITENAME
||    +--database
||    +--source
||    +--static
||    +--virtualenv
