Umee Blockchain Node installation role
=========

This role is intendent to install Umee blockchain node (https://umee.cc/).

Requirements
------------

There is no any special requirement

Role Variables
--------------

- go_path - Path to the GO working directory. Default is `$HOME/work`
- umeed_version - Version of the Umee daemon
- umeed_github_uri - Git URI
- umeed_genesis - URL of the network genesis file
- umeed_genesis_checksum - Checksum of the genesis file
- umeed_seeds - Seed nodes for Umee network
- umeed_persistent_peers - Peer nodes for Umee network
- moniker - Node moniker
- chain_id - Current network Chain Id


Dependencies
------------

In order to run this role you should have go language and `build-essentials` to be installed on the system. You can use `gantsign.golang` to install go language.

Example Playbook
----------------

    ---
    - hosts: umee_hosts
      roles:
        - albertandrejev.umee-node

License
-------

Apache 2.0

Author Information
------------------

Albert Andrejv <a href="mailto:albert.andrejev@gmail.com">albert.andrejev@gmail.com</a>
