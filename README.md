# oh-my-zsh Puppet module

## Overview

This project creates a module used by Puppet to configure a user's account to use
Robby Russell's oh-my-zsh (https://github.com/robbyrussell/oh-my-zsh).

## Usage

Clone this module to your Puppet modules directory (under Puppet this is usually
/etc/puppet/modules.

```
cd /etc/puppet/modules
git clone https://geogit.edina.ac.uk/m.smalll/ohmyzsh-puppet.git ohmyzsh
```

To start using the module from you Puppet manifests:

```
  include ohmyzsh                                                                                                                                                                                                                                                             

  $vagrant = 'vagrant'
  ohmyzsh::setup { "${vagrant}":
    user => "${vagrant}",
  }                                                                                                                                                                                                                                                                          
```
