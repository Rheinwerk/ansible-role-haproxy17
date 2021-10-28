haproxy installation
=========

This role can be used to install haproxy 1.7

[![Build Status](https://github.com/Rheinwerk/ansible-role-haproxy17/actions/workflows/ci.yml/badge.svg)](https://github.com/Rheinwerk/ansible-role-haproxy17/actions/workflows/ci.yml)

Requirements
------------

None.

Role Variables
--------------

There is one main variable that drives this role: `_haproxy`. It is a map that contains all configuration and settings for this role.
Please see `defaults/main.yml` for details.

Dependencies
------------

None.


Example Playbook
----------------

The general contract of this role is to take the variables map `_haproxy` from `defaults/main.yml` as a template for your configuration and pass that configuration as a parameter to this role.

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      var:
        HAPROXY17:
          ...
      roles:
         - { role: haproxy17, tags: [ 'haproxy' ] _haproxy: "{{ HAPROXY17 }}" }

License
-------

Please see LICENSE.

Author Information
------------------

Original author is [Daniel Schneller](https://github.com/dschneller) as member of the [Rheinwerk](https://github.com/Rheinwerk) project.

