bind10
======

This role is for installing bind10 from source. More features will be
added as I use bind10 more.

The installation is based of the instructions from ISC.

Ubuntu: https://bind10.isc.org/wiki/SystemNotesUbuntu1204

I don't use RedHat but there are instructions available from ICS for
both [RHEL and CentOS.](https://bind10.isc.org/wiki/InstallStartPage#RedHatEnterpriseLinuxRHELandderivatives)

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

**Note**: Being in Asia and installing from git isn't a very good
  idea, the ICS repository has really bad connectivity and this might
  be the case for other parts of the world as well. I started out by
  doing it from git but gave up because of how slow it was.

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
