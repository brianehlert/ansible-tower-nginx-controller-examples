# certificates stores in GitHub

Handling Certificates

This demonstration stores the certificate artifacts in a git repository.
With one pull the project downloads the certificates and a set of helper functions.
The file that needs to be updated is the vars.yaml to refer to the correct certificate artifacts.
The rest of the framework playbook should remain the same.

Within Tower:
establish a Project that pulls the repository.
establish a Template that references the project, includes the NGINX Controller credential, and the playbook 'nginx_controller_certificate.yaml'

Here you can also enable a webhook and allow either GitHub ot GitLab to trigger the webhook which will automatically begin the process of updating the certificate stored in NGINX Controller when a check-in to the repository is made.
