---
layout: page
title: Linux Devbox Setup
permalink: /linux
---

This tutorial assumes you are using [Ubuntu](http://www.ubuntu.com/) or some variant like [Xubuntu](http://xubuntu.org/).

## Development Tools

* Install [Atom](https://atom.io/)
* Install Atom plugins: Settings -> Install
  * highlight-selected
  * language-haml
  * language-jade
  * linter
  * linter-eslint
  * minimap
  * trailing-spaces


## The Terminal
* Find and launch your distributions terminal emulator.
* Learn about the command line
  * [Codecademy: Learn the Command Line](https://www.codecademy.com/learn/learn-the-command-line)
* Learn about some common Linux commands by using the `man` command or Google
  * cd
    * What do `~` `.` `..` and `/` refer to?
  * ls
  * grep
  * find
  * ps
  * cat
  * less
  * more
  * vim
  * curl
  * touch
  * sudo
  * su
  * chown
  * chmod
* Learn about combining commands with `|`, `<`, `>`
* Configure your bash profile, Git and SSH
  * **TODO**: find good tutorials on bash, Git and SSH
  * Configure .profile
  * Configure .gitconfig
  * Configure .ssh/config
    * Create a key pair by using `ssh-keygen`
    * Add your public key to GitHub and Bitbucket


## APT and Linux Packages

* Learn about APT. You should be able to:
  * List installed packages
  * Search available packages
  * Update package index
  * Upgrade installed packages
  * Display post-install instructions for an already installed package
* Install Linux build packages (you won't use these directly but they are needed to build and install other software)
  * git-core
  * zlib1g-dev
  * build-essential
  * libssl-dev
  * libreadline-dev
  * libyaml-dev
  * libsqlite3-dev
  * sqlite3
  * libxml2-dev
  * libxslt1-dev
  * libcurl4-openssl-dev
  * python-software-properties
  * libffi-de
* Install Linux packages
  * ack-grep
  * git
  * htop
  * tree
  * wget
  * curl
* Learn about the packages you just installed by using the `man` command or Google


## Ruby, Rails and Jekyll

We are going to use [rbenv](https://github.com/rbenv/rbenv) to install Ruby. This allows you to install multiple versions of Ruby and use different versions for different projects.

* Install [rbenv](https://github.com/rbenv/rbenv) and [ruby-build](https://github.com/rbenv/ruby-build) by following the instructions on their respective pages
* Read the rbenv documentation on [installing Ruby versions](https://github.com/rbenv/rbenv#installing-ruby-versions). You should know how to:
  * List available Ruby versions
  * Install a specific version of Ruby
  * Set a local and global version of Ruby
* Install the latest version of Ruby (2.3.1 at the time of this writing)
* Set the latest version of Ruby as your global default
* Install Rails using `gem install`
  * Checkout and run a Rails project
    * **TODO**: Find a good example Rails app
* Install Jekyll using `gem install`
  * Checkout and run a Jekyll project
    * [This project!](https://github.com/iansu/devbox-setup)


## Node

We are going to use [NVM](https://github.com/creationix/nvm) to install Node. Just like rbenv, NVM allows you to install multiple version of Node and use different versions for different projects.

* Install NVM using the directions listed on their site
* Read the NVM documentation on install Node versions. You should know how to:
  * List available Node versions
  * Install a specific version of Node
  * Set a local and global version of Node
* Install the latest version of Node (6.0.0 at the time of this writing)
* Learn about [NPM](https://www.npmjs.com/), the Node Package Manager
* Install global NPM Packages (`npm install -g`)
  * bower
  * grunt
  * gulp
* Checkout and build a simple Node app
  * **TODO**: Find a good example Node app


## Databases

* Use APT to install the following database packages:
  * postgres
  * mysql
  * sqlite


## Vagrant

Vagrant allows you to easily create virtual machines (VMs) to use for development. Using a VM allows you to run your code in the same version of Linux that is used in production and install project specific versions of software like Ruby, Node, MySQL, Postgres, etc. These development environments are defined in code, which can be checked into version control ensuring everyone is running the exact same environment.

Make sure you install VirtualBox and Vagrant from their respective sites. Do **NOT** use APT to install them.

* Install [VirtualBox](https://www.virtualbox.org/)
* Install [Vagrant](https://www.vagrantup.com/)
* Checkout and run a project based on the Scotch Box
  * **TODO**: Find a good example Vagrant/Scotch Box project


## Future
* Python, Pip and Django
* PHP, Composer and Laravel
* Docker and Docker Compose
