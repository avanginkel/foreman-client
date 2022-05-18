Foreman-client
=========
This is a role to install foreman-clients behind a proxy. Therefore there are a lot of files in the files-directory.

Requirements
------------
Don't forget to download the katello-ca-consumer.rpm from your foreman-server. And copy this to your files/folder. For example: files/Rocky/8/
This role installs a lot of files that are necesary to install the katello package.

It is possible that packages still are missing. If so, please tell me.

Role Variables
--------------

- organization  _What organization is defined in foreman_
- installationfiles: /tmp/rpms
- repodir: _/etc/yum.repos.d/_ or _/etc/apt/sources.list.d/_

_Activationkeys defined in foreman_
- activationkeyota: 
- activationkeyprod: 

_Puppet environment defined in foreman_
- environmentota: 
- environmentprod:

_Which hostgroups defined in foreman_ 
- hostgroupota: for example: Centos7/OTA
- hostgroupprod: 

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

- MIT

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).

