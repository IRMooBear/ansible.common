Common
=========

This is a common role that Anh Nguyen run before all other roles to setup some things on servers.

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

    install_aws_cli: no

Whether or not to install AWS CLI

    aws_cli_output: text
    aws_region: us-west-2
    aws_access_key_id:
    aws_secret_access_key:
    
Configuration variables in case AWS cli is installed.    

    smtp_relay:

Configure sendmail for SMTP relay on Raspberry Pi or other servers at home.  Leave blank on real servers.

    email:
    
Email of the server admin to forward emails to.    

Example Playbook
----------------
    - hosts: servers
      roles:
         - { role: irmoobear.common }

License
-------
BSD

Author Information
------------------
An optional section for the role authors to include contact information, or a website (HTML is not allowed).