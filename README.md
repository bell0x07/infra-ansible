This ansible playbook is to be used for bell's personal machines
----------------------------------------------------

## Ansible configuration:
1. Install ansible from
https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html#installing-the-control-machine

2. Download and extract mitogen in /opt/
https://files.pythonhosted.org/packages/source/m/mitogen/mitogen-0.2.3.tar.gz

## Usage:

0. First run should be done for a specific host, as user root

`ansible-playbook --user root --ask-pass site.yml -l jenkinsarkadiusz`

1. Deploy to specific host or groups of hosts

`ansible-playbook --user agluszyk site.yml -l jenkinsarkadiusz`

2. Deploy to all hosts in inventory:

`ansible-playbook --user agluszyk site.yml`

you can also leave the `--user` option out, if you have correct unix username, or correct user configured in ~/.ssh/config
# infra-ansible
