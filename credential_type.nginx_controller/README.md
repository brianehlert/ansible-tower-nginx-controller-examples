# NGINX Controller Credential Type

To define a new Cloud credential type of NGINX Controller is Ansible Tower and to support the use of the Ansible Role nginxinc.nginx_controller_generate_token; do the following:

In Ansible Tower:

Select credential types under the Administration section
Select '+' to add a new Credential Type
Name the credential type 'NGINX Controller'
For the INPUT CONFIGURATION section copy and paste from the file input_configuration.yaml
For the INJECTOR CONFIGURATION section copy and paste from the file injector_configuration.yaml
Select Save

Select the Credentials section under Resources
Select '+' to add a new Credential
Provide a name that is logical for the NGINX Controller instance in your organization
Set the Organization that is allowed to use the credential
In the CREDENTIAL TYPE field search for 'NGINX Controller' (the name of the type defined above)
Enter the user email for the NGINX Controller account to use with Ansible
Enter the user password for the account
Enter the DNS Hostname or IP address of the NGINX Controller instance.
Select save.

This Credential can now be used in conjunction with the nginxinc.nginx_controller_generate_token Role that you can include in your playbooks prior to invoking other Roles such as nginxinc.nginx_controller_component or nginxinc.nginx_controller_gateway