# Ansible playbooks for deploying a Mezzanine application(with roles and multi machines)

This code shows how to use Ansible to deploy a Mezzanine site into a Vagrant box.

Change the pip.conf to accerlerate the pip install speed.

## Before running the playbook

Don't forget to change the Vagrant box in Vagrantfile to locally-added box(Ubuntu 14) or ubuntu/trusty64

## Running the playbook

Then you can deploy Mezzanine by doing:

    vagrant up
    ansible-playbook mezzanine-across-hosts.yml


Then point your browser to: <http://192.168.2.11.xip.io> or
<https://www.192.168.2.11.xip.io>. You'll get a security warning if you use the
https site since it's a self-signed certificate, this is normal.
