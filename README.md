DNS
=========

Installation and configuration of dnsmasq for use in a small network

Requirements
------------

Create first a machine with a static ip and a hostname related to dns (*ns1* is a good one ?).

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Installation :
Create file "requirements.yml" with this information :

```yaml
---
- src: https://github.com/watysay/ansible-role-dns.git
  scm: git
  version: main
  name: dns
```
and install with 
```sh
ansible-galaxy install -r requirements.yml
```
(add -f roles if needed)


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

GPL v3

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
