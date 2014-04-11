ansible-aws-examples
====================

Example playbooks to launch AWS infrastructure.

Steps:

1. Edit vars/aws-creds.yml to include your own AWS credentials
2. Edit vars/dev-environment.yml to define the security groups,
   sets of instances, etc, that will be used.
3. Run: ansible-playbook -i hosts provision.yml

You can shut down the infrastructure by setting the exact_count values
in the vars/dev-environment.yml file to 0 and re-running provision.yml.
