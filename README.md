Role Name
=========

Role to create ssh configuration when a proxy is needed.

Requirements
------------

None.

Role Variables
--------------

- **ekara_ssh_proxy**: proxy url. Example: http://user:password@myproxy.com:80
- **ekara_ssh_key**: SSH private key file.
- **ekara_ssh_host**: Host pattern for proxy configuration. 


Dependencies
------------

None.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
    	tasks:
		  include_role:
		    name: ekara.ssh
		  vars:
		    ekara_ssh_proxy: 'http://user:password@proxy.com:80'
		    ekara_ssh_key: /opt/mykey.pem
		    ekara_ssh_host: '*.xxx.com'

License
-------

MITs

Author Information
------------------

https://github.com/ekara-platform/ansible-role-ssh-config.git
