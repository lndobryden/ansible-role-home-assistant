[![Build Status](https://travis-ci.org/lndobryden/ansible-role-home-assistant.svg?branch=master)](https://travis-ci.org/lndobryden/ansible-role-home-assistant)
Ansible Role for Home Assistant
=========

An Ansible role for installing Home assistant in a docker container
Works with Aeotec usb zwave controller

Requirements
------------

Requires Docker to be installed

Role Variables
--------------

```
aws_access_key_id:
aws_secret_access_key:
aws_region:
latitude:
longitude:
elevation:
time_zone:
darksky_api_key:
zwave_network_key:
```

Example Playbook
----------------

```
    - hosts: servers
      roles:
      - { role: home-assistant,
          aws_access_key_id: key,
          aws_secret_access_key: key,
          aws_region: us-east-1,
          latitude: 12.345,
          longitude: -12.345,
          elevation: 12345,
          time_zone: America/Los_Angeles,
          darksky_api_key: 12345,
          zwave_network_key: "0x1, 0x2, 0x3, 0x4, 0x5, 0x6, 0x7, 0x8, 0x9, 0xA, 0xB, 0xC, 0xD, 0xE, 0xF, 0x1" }

```
License
-------

BSD

Author Information
------------------

Lee Dobryden - https://github.com/lndobryden
