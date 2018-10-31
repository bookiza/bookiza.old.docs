---
layout: post
title:  "Installation"
date:   2018-10-30 10:15:00 -0000
categories: bookiza installation steps
---

Bookiza is super easy to install. 

The following dependencies must be installed before proceeding to install Bookiza.

> node (>=8.11.3), gulp, shelljs, git-scm and a unixy-style shell or the terminal app.


### Install Nodejs

It is recommended to install the latest stable (it's free!) version of node (v8.11.3 or higher as of writing this) directly from the [Nodes.js® website](https://nodejs.org/en/download/). 


#### Mac/ El Capitan

On Mac it is generally recommended to install use [homebrew](http://brew.sh/) to install node. Also works with Linux/Ubuntu. 


```bash
$ ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
$ brew update
$ brew doctor

```

Once your system is ready to brew, install node:
```bash
$ brew install node 
```
When node installation is over, check: 

```bash
$ node -v
v10.6.0

```


#### Windows
Download the Windows installer and run the installer (the .msi file) in the previous step. Follow the prompts in the installer, accept the license agreement, click the NEXT button to accept the default installation settings. 

Restart your computer.

#### Linux
Use package control to grab the appropriate [node installer](https://nodejs.org/en/download/package-manager/) for your distro. You can use `homebrew` to install node on a linux machine.

Once node is installed always check its version with:

`$ node -v`


Next, we'll install `git`.


---


### GIT-SCM

Bookiza uses the [git-scm](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) internally to hook up your project (manuscript) to a repository. While this step is not mandatory, it is highly recommended to commit and track changes to your manuscript over time and check-in the progress into a repository on sites like [Github](https://github.com) or [Bitbucket](https://bitbucket.org) to back it up. 

You can use any other version control software if you like. 

#### Mac / El Capitan

If you are using Mac, you may already have Git. To find out, open a terminal and enter `git --version`. If it's not there already, install with `brew install git`.

Or you can [download](http://git-scm.com/downloads) the installer, double-click the `.dmg` and complete its installation. After installation is complete, configure git `global user.name` and `global user.email` on your machine as shown below:


```
$ git --version
$ git version 2.10.1
```


> Configure git after installation with:

```
$ git config --global user.name "Your Full Name"

$ git config --global user.email "your@email.com"

```



#### Windows

Download the [Windows Installer Package](http://git-scm.com/download/win) for Git.

Run the installer on your computer to open Git Setup wizard and follow through all the steps to complete the installation. Once the installation has completed, open `Bash.vbs` inside the Git folder / Programs directory to open the command window.

Configure your Git `global user.name` and Git `global user.email` as shown above.

#### Linux / Ubuntu

On Ubuntu use the apt package manager or the command line utility `apt-get` (or optionally the GUI like Synaptic or Aptitude) to install Git. 
You can also install `git` via the terminal with one of the following commands depending on your distro:

```bash
$ brew install git          # Works on Mac & Linux both.
```
Or,

```bash
$ sudo apt-get install git  # Ubuntu/Debian 
```
Or, 

```bash
$ sudo yum install git-all  # Fedora

```

Upon completion of installation make sure to configure Git `global user.name` and `global user.email` as shown above.

---


### Install Bookiza

You'll need to install `bookiza` and `gulp` globally. Once the installation is complete, check with `$ bookiza --version`.

```
$ npm install bookiza@1.0.0-beta.4 -g      // Or $ npm i bookiza@latest -g

$ bookiza --version
1.0.0-beta.4

$ bookiza --help        // Glossary

```



> If for some reason you're unable to upgrade node binaries (for example, on v6.2.0 or below) you might want to try installing bookiza as-is first and if it doesn't work then use the `\--harmony` flag in the shebangs of the executable <a href="https://github.com/bookiza/bookiza/blob/master/bin/bin.js">bin</a>. 
> Read more about this <a href="http://stackoverflow.com/questions/28756759/how-to-start-global-npm-module-with-harmony-flag"> issue</a> on Stackoverflow. 

##### Dependencies
async, superagent, progress, co-prompt, co, path, fs, chalk, commander, string, dateformat, shelljs, os-homedir

> The <a href="https://github.com/bookiza/bookiza/blob/master/bash/.bookiza">bash plugin </a> of Bookiza has been deprecated. 

