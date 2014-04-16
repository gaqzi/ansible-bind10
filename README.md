bind10
======

This role is for installing bind10 from source. More features will be
added as I use bind10 more.

Requirements
------------

None

Role Variables
--------------

Toggles:

* `bind10_build_dhcp`: **no** - whether bind should be built with DHCP support
* `bind10_install_manpages`: **no** - whether manpages should be installed
* `bind10_force_reinstall`: **no** - whether bind should be recompiled and installed
* `bind10_from_git`: **no** - whether to download bind from git
* `bind10_from_file`: **yes** - whether to download bind as a file

Configurables:

* `bind10_prefix_path`: **/usr/local** - where bind will be installed
* `bind10_version`: **1.1.0** - which version to install

Dependencies
------------

None

Example Playbook
-------------------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: gaqzi.bind10 }

License
-------

BSD

Author Information
------------------

Björn Andersson - @gaqzi.
