Role Name
=========

Role to create ssh configuration when a proxy is needed.

Requirements
------------

None.

Role Variables
--------------

- **lagoon_ssh_proxy**: proxy url. Example: http://user:password@myproxy.com:80
- **lagoon_ssh_key**: SSH private key file.
- **lagoon_ssh_host**: Host pattern for proxy configuration. 


Dependencies
------------

None.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
    	tasks:
		  include_role:
		    name: lagoon.ssh
		  vars:
		    lagoon_ssh_proxy: 'http://user:password@proxy.com:80'
		    lagoon_ssh_key: /opt/mykey.pem
		    lagoon_ssh_host: '*.xxx.com'

License
-------

MITs

Author Information
------------------

https://github.com/lagoon-platform/ansible-role-ssh-config.git
