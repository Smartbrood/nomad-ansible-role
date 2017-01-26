consul-ansible-role
===================
[![Build Status](https://travis-ci.org/Smartbrood/nomad-ansible-role.svg?branch=master)](https://travis-ci.org/Smartbrood/nomad-ansible-role)

Setup Nomad by HashiCorp.


Caveats
-------

* Currently deb packages url points to custom site
* validate_certs=no in get_url module due to lack of SNI support in Ubuntu 14.04 



Role Variables
--------------




Example Playbook
----------------

ansible-galaxy install -r requirements.yml 

    - hosts: servers
      roles:
         - { role: nomad, nomad_mode: client }


License
-------

Apache License Version 2.0


Author Information
------------------

Andrey N. Petrov <andreynpetrov@gmail.com>
