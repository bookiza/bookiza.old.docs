---
layout: post
title:  "Installation"
date:   2018-07-26 17:16:51 -0400
categories: bookiza installation steps
---

### Install Nodejs

Recommended Node v6.2.0 or above. 

It is recommended to install the latest stable (It's FREE!) version of node (v6.2.0 as of writing this) directly from the [Nodes.js® website](https://nodejs.org/en/download/). 


#### Mac/ El Capitan

```
$ ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
$ brew update
$ brew doctor

$ brew install node 
```
> Once node is installed check with $ node -v

On Mac it is generally recommended to install nodejs with [Homebrew](http://brew.sh/) (Instructions on right). 

Once your system is ready to brew, install node with

`$ brew install node`


#### Windows
Download the Windows installer and run the installer (the .msi file) in the previous step. Follow the prompts in the installer, accept the license agreement, click the NEXT button to accept the default installation settings. 

Restart your computer.

#### Linux
Use package control to grab the appropriate [node installer](https://nodejs.org/en/download/package-manager/) for your distribution of linux.

Once node is installed on your machine check its version with:

`$ node -v`

---


### Install GIT

```
$ git --version
$ git version 2.10.1
```

```
$ brew install git      # Mac

$ sudo apt-get install git  # Ubuntu/Debian 

$ sudo yum install git-all  # Fedora

```

> Configure git after installation with:

```
$ git config --global user.name "Your Full Name"

$ git config --global user.email "your@email.com"

```



Internally Bookiza utilizes [git-scm](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) to hook up your manuscript to a repository. While this is not mandatory, it is highly recommended to check-in your manuscript into a repository like [Github](https://github.com) or [Bitbucket](https://bitbucket.org) and back it up. You can use any other version control software if you like. 

#### Mac / El Capitan

If you are using Mac, you may already have Git. To find out, open a terminal and enter `git --version`. If it's not there already install with `brew install git`.

Or you can [download](http://git-scm.com/downloads) the installer, double-click the dmg and complete its installation. After installation is completed configure Git `global user.name` and `global user.email` as shown on the right.


#### Windows

Download the [Windows Installer Package](http://git-scm.com/download/win) for Git.

Run the installer on your computer to open Git Setup wizard and follow through all the steps to complete the installation. Once the installation has completed, open `Bash.vbs` inside the Git folder / Programs directory to open the command window.

Configure your Git `global user.name` and Git `global user.email` as shown on the right.

#### Linux / Ubuntu

On Ubuntu use the apt package management system or the command line utility `apt-get` (or optionally the graphical user interfaces like Synaptic or Aptitude) to install Git. 

Upon completing installation make sure to configure Git `global user.name` and `global user.email` as shown alongside.

---


### Install Bookiza

```
$ npm install bookiza -g

$ bookiza -v

1.0.1

$ bookiza --help        // See help/options/documentation

```

On your terminal run:

`$ npm install bookiza -g`

You'll need to install `bookiza` and `gulp` globally. Once the installation has completed, check with `$ bookiza --version`.

<aside class="notice"> 
  <span>
    If for some reason cannot upgrade to node v6.2.0 (or above) you might want to try bookiza as-is first with a slightly older version of node. If it doesn't work then try using the `\--harmony` flag in the shebangs of the executable <a href="https://github.com/bookiza/bookiza/blob/master/bin/bin.js">bin</a>. 
  </span>

  <p> 
    <br/> Read more about this <a href="http://stackoverflow.com/questions/28756759/how-to-start-global-npm-module-with-harmony-flag"> issue</a> on Stackoverflow. </p>
</aside>

##### Dependencies
async, superagent, progress, co-prompt, co, path, fs, chalk, commander, string, dateformat, shelljs, os-homedir

<aside class="warning"> The <a href="https://github.com/bookiza/bookiza/blob/master/bash/.bookiza">bookiza bash plugin </a> is now deprecated. 
</aside>
