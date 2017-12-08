memoryleak.pound
=========

Simple Pound installation

Requirements
------------

You need to make sure that for RHEL based distros EPEL is installed and enabled.

Role Variables
--------------

	pound_service: pound
	pound_log_level: 3
	pound_listen_http_address: 0.0.0.0
	pound_listen_http_port: 443
	pound_backend_servers: 
	  - [ '127.0.0.1', '80' ]

Dependencies
------------

No dependencies.

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: memoryleak.pound }

License
-------

BSD

Author Information
------------------

Haydar Ciftci <haydar.ciftci@gmail.com>