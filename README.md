# EXIM Public ('exim-public')

**Part of the BAS Ansible Role Collection (BARC)**

Installs the EXIM Mail Transfer Agent

## Overview

* Installs EXIM MTA.
* Configures EXIM to use BAS Cambridge smart host.

## Availability

This role is designed for internal use but if useful can be shared publicly.

## Usage

### Requirements

#### BAS Ansible Role Collection (BARC)

* `core`

### Variables

* `exim_dc_smarthost`
    * Default: "" (empty string)
* `xim_dc_other_hostnames`
    * Default: "{{ ansible_hostname }}""
* `exim_dc_readhost
    * Default: "" (empty string)
* `exim_dc_config_type
    * Default: "smarthost"
* `exim_dc_local_interfaces
    * Default: "" (empty string)
* `exim_dc_localdelivery
    * Default: "mail_spool"
* `exim_dc_relay_domains
    * Default: "" (empty string)
* `exim_dc_relay_nets
    * Default: "" (empty string)
* `exim_dc_minimal_dns
    * Default: "false"
* `exim_dc_mailname_in_oh
    * Default: "true"
* `exim_dc_hide_mailname
    * Default: "true"
* `exim_dc_use_split_config:
    * Default: "false"
* `exim_cfilemode
    * Default: "644"

## Contributing

This project welcomes contributions, see `CONTRIBUTING` for our general policy.

## Developing

### Committing changes

The [Git flow](https://github.com/fzaninotto/Faker#formatters) workflow is used to manage development of this package.

Discrete changes should be made within *feature* branches, created from and merged back into *develop* (where small one-line changes may be made directly).

When ready to release a set of features/changes create a *release* branch from *develop*, update documentation as required and merge into *master* with a tagged, [semantic version](http://semver.org/) (e.g. `v1.2.3`).

After releases the *master* branch should be merged with *develop* to restart the process. High impact bugs can be addressed in *hotfix* branches, created from and merged into *master* directly (and then into *develop*).

### Issue tracking

Issues, bugs, improvements, questions, suggestions and other tasks related to this package are managed through the BAS Web & Applications Team Jira project ([BASWEB](https://jira.ceh.ac.uk/browse/BASWEB)).

## License

Copyright 2015 NERC BAS. Licensed under the MIT license, see `LICENSE` for details.
