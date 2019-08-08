Role Name
=========

Role to create and maintain SSH configuration with or without proxy.

Requirements
------------

None.

Role Variables
--------------

- **ek_ssh_key**: SSH private key file.
- **ek_ssh_host**: Host pattern for proxy configuration.
- **ek_ssh_proxy**: Optional proxy url for SSH connection. Example: http://user:password@myproxy.com:80


Dependencies
------------

None.

Example Playbook
----------------

    - hosts: localhost
    	tasks:
		  include_role:
		    name: ekara.ssh
		  vars:
		    ek_ssh_proxy: 'http://user:password@proxy.com:80'
		    ek_ssh_key: /opt/mykey.pem
		    ek_ssh_host: '*.xxx.com'

License
-------

MIT

Author Information
------------------

https://github.com/ekara-platform/ansible-role-ssh-config.git
