# NGINX Controller Ansible Tower Examples

This repository is a set of examples built around using Ansible Tower with the NGINX Controller Collection.

These are demo examples designed to get you started.
These resources are open to more scenarios as folks need them.  Just open an issue or build a scenario and issue a pull request against the repository.
I hope you find a useful pattern in this set of examples.

## credential_type.nginx_controller

Establishing a cloud credential type for NGINX Controller that is compatible with the Roles in the Collection.

## certificate_merch.acmefinancial.net

A demonstration repository of storing certificates in a repository and using a playbook and the Roles in Ansible Tower to update the certificate stored in NGINX Controller.

## Controller Gateway instances

A demonstration repository for deploying new instances in AWS, installing NGINX Plus, installing the NGINX Controller Agent, then removing the special inventory tag.

## gateway_

Maintaining your NGINX Controller gateway configuration in source control and using a single Ansible Tower Template to push your gateway configurations to Controller.

## requirements.yml

One pattern that is used and repeated is the use of requirements.yml for each playbook.
The flexibility of this is pretty powerful for both Roles and Collections as you can select multiple sources and easily switch between development and production for example.
There is more here: https://galaxy.ansible.com/docs/using/installing.html
