# Ansible PlayBook for Norikra Server and td-agent

## Requirement
 - Python-2.6 or 2.7
 - Ansible 2.x higher 
 
## Install
 - git clone
 - edit playbooks as you like 
   - update development/staging/production inventory file for YOUR enveriorments
   - update host_vars/{{ "STAGING" }}.yml
   - update roles if you need
   - ... and so on

## Usage (PlayBook)
 - Setup SSH connectivity from YOUR Ansible node to "Targets" in inventory.
 - "ansible ping" maybe your help.
 ```
 $ ansible <SOMEWHERE YOUR NODE> -m ping
 ```
 - "ansible --syntax-check" also helpfull.
 ```
 $ ansible-playbook -i staging norikra.yml --syntax-check
 ```
 - do it
  ```
 $ ansible-playbook -i staging norikra.yml
 ```
 
# Copyright
* Copyright:: Copyright (c) 2017- endless pancake
* License::   Apache License, Version 2.0
