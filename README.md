Protection Profile for General Purpose Operating Systems
=========

[![Build Status](https://travis-ci.org/RedHatOfficial/ansible-role-rhel8-ospp.svg?branch=master)](https://travis-ci.org/RedHatOfficial/ansible-role-rhel8-ospp)
[![Ansible Role](https://img.shields.io/ansible/role/40355.svg)](https://galaxy.ansible.com/RedHatOfficial/rhel8-ospp-role)
[![GitHub release](https://img.shields.io/github/release/RedHatOfficial/ansible-role-rhel8-ospp.svg)](https://github.com/RedHatOfficial/ansible-role-rhel8-ospp/releases/latest)

Ansible Role for profile ospp for General Purpose Operating Systems

Profile Description:  
This profile reflects mandatory configuration controls identified in the  
NIAP Configuration Annex to the Protection Profile for General Purpose  
Operating Systems (Protection Profile Version 4.2).  

The tasks that are used in this role are generated using OpenSCAP.
See the OpenSCAP project for more details on Ansible playbook generation at [https://github.com/OpenSCAP/openscap](https://github.com/OpenSCAP/openscap)

To submit a fix or enhancement for an Ansible task that is failing or missing,
see the ComplianceAsCode project at [https://github.com/ComplianceAsCode/content](https://github.com/ComplianceAsCode/content)

## Requirements

- Ansible version 2.5 or higher

## Role Variables

To customize the role to your liking, check out the [list of variables](vars/main.yml).

## Dependencies

N/A

## Example Playbook

Run `ansible-galaxy install RedHatOfficial.rhel8_ospp` to
download and install the role. Then, you can use the following playbook snippet to run the Ansible role:

    - hosts: all
      roles:
         - { role: RedHatOfficial.rhel8_ospp }

Next, check the playbook using (on the localhost) the following example:

    ansible-playbook -i "localhost," -c local --check playbook.yml

To deploy it, use (this may change configuration of your local machine!):

    ansible-playbook -i "localhost," -c local playbook.yml

## License

BSD-3-Clause

## Author Information

This Ansible remediation role has been generated from the body of security
policies developed by the ComplianceAsCode project. Please see
[https://github.com/complianceascode/content/blob/master/Contributors.md](https://github.com/complianceascode/content/blob/master/Contributors.md)
for an updated list of authors and contributors.
