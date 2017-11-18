## galaxy-role-default/default

[![Travis CI](http://img.shields.io/travis/csteel/ansible-rolegalaxy-role-default/default.svg?style=flat)](http://travis-ci.org/csteel/ansible-rolegalaxy-role-default/default)
[![Platforms](http://img.shields.io/badge/platforms-debian%20/%20ubuntu-lightgrey.svg?style=flat)](#)

This is a drop in replacement role skeleton used to create ansible roles with the ansible-galaxy command.

List of internal variables used by the role:

    fact_controller_home
    fact_controller_user

### Usage

#### Create role on github or other git server

```shell
ansible-role-fetch
```

#### Clone empty role locally

#### Create role using this role

Use the roles short name. for example:

```shell
fetch
```

using one of the following methods:

You can replace the default ansble-galaxy role skeleton or point to this one using the ansible-galaxy ROLE_SKELETON option.

#### To use as an alternative role skeleton

```shell
ansible-galaxy init --role-skeleton=ALTERNATIVE_ROLE_SKELETON_PATH ansible-role-myrole
```

Real world example

```shell
mkdir ~/projects
cd ~/projects
git clone git@github.com:cjsteel/galaxy-role-default.git
ansible-galaxy init --role-skeleton=/home/cjs/projects/galaxy-role-default/skeleton -f ansible-role-download -vvv
```

#### Replacing the ansible galaxy default role template

```shell
cd ~/miniconda2/envs/ansible/lib/python2.7/site-packages/ansible/galaxy/data/default
mv default default.org
git clone git@github.com:cjsteel/galaxy-role-default.git default
```

### Authors and license

- [Christopher Steel](http://mcin-cnim.ca/) | [e-mail](mailto:christopher.steel@mcgill.ca)

License: [MIT](https://tldrlegal.com/license/mit-license)

### Open Science

The Neuro has adopted the principles of Open Science. We are inspired by the likes of the Allen Institute for Brain Science, the National Institutes of Health's Human Connectome project, and the Human Genome project. For additional information please see [open science at the neuro](https://www.mcgill.ca/neuro/open-science-0).

![MCIN](skeleton/imgs/mcin-logo-brain-140x116.png)          ![neuro](skeleton/imgs/neuro-logo-160x116.png)  

