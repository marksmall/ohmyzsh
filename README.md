#ohmyzsh

####Table of Contents

1. [Overview](#overview)
2. [Module Description - What the module does and why it is useful](#module-description)
3. [Setup - The basics of getting started with ohmyzsh](#setup)
    * [What ohmyzsh affects](#what-ohmyzsh-affects)
    * [Setup requirements](#setup-requirements)
    * [Beginning with ohmyzsh](#beginning-with-ohmyzsh)
4. [Usage - Configuration options and additional functionality](#usage)
5. [Reference - An under-the-hood peek at what the module is doing and how](#reference)
5. [Limitations - OS compatibility, etc.](#limitations)
6. [Development - Guide for contributing to the module](#development)

##Overview

Decorate specified **User Accounts** with Robby Russell's **oh-my-zsh**
ZSH Framework (https://github.com/robbyrussell/oh-my-zsh).

##Module Description

This module ensures that:

1. **ZSH** is installed and set as the default shell used by the specified **User**.  
2. **GIT** is installed.

The module clones a copy of oh-my-zsh from https://github.com/robbyrussell/oh-my-zsh
to the user's home directory and adds a pre-defined custom theme and *.zshrc* file.

##Setup

###What ohmyzsh affects

* package files for **ZSH** and **GIT**.
* User's **.zshrc** file.
* */etc/passwd* file (defines what the user's default shell should be).

###Setup Requirements **OPTIONAL**

NOTHING. 
	
###Beginning with ohmyzsh	

To begin using the ohmyzsh module:

```include ohmyzsh```

```
$vagrant = 'vagrant'
  $root = 'root'

  ohmyzsh::setup { "${vagrant}":
    user => "${vagrant}",
  }

  ohmyzsh::setup { "${root}":
    user => "${root}",
  }
```

##Usage

NOTHING. 

##Reference

NOTHING.

##Limitations

This module has only been tested on CentOS-6.4-x64

##Development

This module is an open project, community involvement is welcome in ensuring this 
module stays current.

We want to keep it as easy as possible to contribute changes so that our modules 
work in your environment. There are a few guidelines that contributors should 
follow so that we can have a chance of keeping on top of things.  We are happy to
follow the guidlines Puppet Labs themselves have developed at [Puppet Labs wiki](http://projects.puppetlabs.com/projects/module-site/wiki/Module_contributing).

##Release Notes/Contributors/Etc **Optional**

If you aren't using changelog, put your release notes here (though you should consider using changelog). You may also add any additional sections you feel are necessary or important to include here. Please use the `## ` header. 
