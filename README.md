Team and repository tags
========================

<!-- Change things from this point on -->

ssdb
=======

#### Table of Contents

1. [Overview - What is the ssdb module?](#overview)
2. [Module Description - What does the module do?](#module-description)
3. [Setup - The basics of getting started with ssdb](#setup)
4. [Implementation - An under-the-hood peek at what the module is doing](#implementation)
5. [Limitations - OS compatibility, etc.](#limitations)
6. [Development - Guide for contributing to the module](#development)
7. [Contributors - Those with commits](#contributors)

Overview
--------

The puppet-ssdb module is used to manage deployment of SSDB. SSDB is a high performace key-value(key-string, key-zset, key-hashmap) NoSQL database, an alternative to Redis.

Module Description
------------------

The ssdb module is a thorough attempt to make Puppet capable of managing the entirety of ssdb.

Setup
-----

**What the ssdb module affects**

* [ssdb](https://github.com/ideawu/ssdb), high performace key-value(key-string, key-zset, key-hashmap) NoSQL database.

### Installing ssdb

    ssdb is not currently in Puppet Forge, but is anticipated to be added soon.  Once that happens, you'll be able to install ssdb with:
    puppet module install newptone/ssdb

### Beginning with ssdb

To utilize the ssdb module's functionality you will need to declare multiple resources.

Implementation
--------------

### ssdb

ssdb is a combination of Puppet manifest and ruby code to delivery configuration and extra functionality through types and providers.

Limitations
------------

* All the ssdb types use the CLI tools and so need to be ran on the ssdb node.

Beaker-Rspec
------------

This module has beaker-rspec tests

To run the tests on the default vagrant node:

```shell
bundle install
bundle exec rake acceptance
```

For more information on writing and running beaker-rspec tests visit the documentation:

* https://github.com/puppetlabs/beaker-rspec/blob/master/README.md

Development
-----------

Please follow Developer documentation for the entire puppet-openstack project.

* http://docs.openstack.org/developer/puppet-openstack-guide/

Contributors
------------

* https://github.com/newptone/puppet-ssdb/graphs/contributors
