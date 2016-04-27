---
layout: page
title: Mac Devbox Setup
permalink: /mac
---

## Development Tools

* Install Xcode from the Mac App Store
  * https://itunes.apple.com/ca/app/xcode/id497799835
* Install Atom: https://atom.io/
* Install Atom plugins: Settings -> Install
  * highlight-selected
  * language-haml
  * language-jade
  * linter
  * linter-eslint
  * minimap
  * trailing-spaces


## The Terminal
* Install iTerm or configure Terminal.app (in `/Applications/Utilities`)
* Learn about the command line
  * **TODO**: find a good linux command line tutorial
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
* Configure your bash profile, Git and SSH
  * **TODO**: find good tutorials on bash, Git and SSH
  * Configure .bash_profile
  * Configure .gitconfig
  * Configure .ssh/config
    * Create a key pair by using `ssh-keygen`


## Homebrew and Linux Packages

* Install Homebrew: http://brew.sh/
* Learn about homebrew commands. You should be able to:
  * List installed packages
  * Search available packages
  * Update homebrew
  * Upgrade installed packages
  * Display post-install instructions for an already installed package
* Install Linux packages
  * ack
  * git
  * htop-osx
  * tree
  * wget
* Make sure to read the post-install intructions that homebrew displays for each package. Some packages require additional configuration to work properly.
* Learn about the packages you just installed by using the `man` command or Google


## Ruby, Rails and Jekyll

We are going to use [rbenv](https://github.com/rbenv/rbenv) to install Ruby. This allows you to install multiple versions of Ruby and use different versions for different projects.

* Install rbenv using homebrew by installing the following packages
  * rbenv
  * rbenv-gem-rehash
  * ruby-build
* Read the rbenv documentation on [installing Ruby versions](https://github.com/rbenv/rbenv#installing-ruby-versions). You should know how to:
  * List available Ruby versions
  * Install a specific version of Ruby
  * Set a local and global version of Ruby
* Install the latest version of Ruby (2.3.0 at the time of this writing)
* Set the latest version of Ruby as your global default
* Install Rails using `gem install`
  * Checkout and run a Rails project
    * **TODO**: Find a good example Rails app
* Install Jekyll using `gem install`
  * Checkout and run a Jekyll project
    * This project!


## Node

We are going to use NVM to install Node. Just like rbenv, NVM allows you to install multiple version of Node and use different versions for different projects.

* Install NVM using homebrew
* Read the NVM documention on install Node versions. You should know how to:
  * List available Node versions
  * Install a specific version of Node
  * Set a local and global version of Node
* Install the latest version of Node
* Install NPM Packages
  * bower
  * grunt
  * gulp
  * jasmine?
  * phantomjs?
* Checkout and build a simple Node app
  * **TODO**: Find a good example Node app


## Databases

* Use homebrew to install the following database packages:
  * postgres
  * mysql
  * sqlite
* Configure MySQL and Postgres to start on boot by following the homebrew post-install instructions


## Vagrant

Vagrant allows you to easily create virtual machines (VMs) to use for development. Using a VM allows you to run your code in the same version of Linux that is used in production and install project specific versions of software like Ruby, Node, MySQL, Postgres, etc. These development environments are defined in code, which can be checked into version control ensuring everyone is running the exact same environment.

* Install VirtualBox
* Install Vagrant
* Checkout and run a project based on the Scotch Box
  * **TODO**: Finda  good example Vagrant/Scotch Box project


## Future
* Python, Pip and Django
* PHP, Composer and Laravel
* Docker and Docker Compose
