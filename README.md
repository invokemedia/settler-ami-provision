Invoke AMI
==========

This is the anisble role used to create the Invoke AMI. It is basically a snapshot of the [invokemedia/ansible-laravel-settler](https://github.com/invokemedia/ansible-laravel-settler) project.

See the AMI info with `aws ec2 describe-images --image-ids ami-f4599394`.

### Installation

* Clone this repo
* create an `inventory` file with the ip and user for the server you want to provision
* run `ansible-playbook playbook.yml -i inventory`

### Updating the AMI

* all the steps above then,
* when that is complete, go to the EC2 panel and create an image for the server

### What's Included

* PHP7
  * bcmath
  * intl
  * mcrypt
  * readline
  * zip
  * apcu
  * curl
  * gd
  * imap
  * mbstring
  * memcached
  * mysql
  * pgsql
  * soap
  * sqlite3
  * xml
* Composer
* Nginx
  * php-fpm
* git
* python
* supervisor
* a few other essentials...
