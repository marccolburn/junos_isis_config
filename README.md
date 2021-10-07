IS-IS Configuration
=========

Configure IS-IS for Junos.

Requirements
------------


Role Variables
--------------
isis_interfaces: List of Dictionaries containing IS-IS interfaces and unit
* name: Name of physical interface, string
* unit: unit of interface, int

isis_settings: Dictinary containing settings for IS-IS
* loopback_unit: unit of interface, int
* loopback_clns_address: clns address of loopback, string
* level1_disable: level1 disabled or enabled, boolean value

Dependencies
------------

N/A

Example Playbook
----------------

    - hosts: all
      roles:
         - { role: junos_isis_config }

License
-------

BSD

Author Information
------------------

Marc Colburn Juniper
