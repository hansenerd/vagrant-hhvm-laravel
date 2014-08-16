# ansible play for installing HipHopVM and laravel

This sets up a vagrant box (debian wheezy), and
installs nginx, hhvm and laravel.

## requirements

* [VirtualBox](https://www.virtualbox.org/) + [Vagrant](http://www.vagrantup.com/)
* [ansible](http://docs.ansible.com/intro_installation.html)

## usage

Just run `vagrant up` and wait. After installation you will have a `laravel/` folder
in the current directory, served at http://localhost:8080/.

adapted from [this blog](http://fideloper.com/hhvm-nginx-laravel).
