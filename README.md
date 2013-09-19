Ansible / redis
===============

Ansible playbook to install and setup a Redis upstart service.



Usage
-----

Create an inventory file with the servers that you want to Node.js on or use `$ANSIBLE_HOSTS`.

if connecting with root:

    ansible-playbook -i inventory-file -u root main.yml

if sudoing:

    ansible-playbook -i inventory-file -K main.yml

It installs a `redis-local` script that is useful to use instead of `redis-cli` if you set a different port and password.



Ansible
-------

Not sure what Ansible is? Read the getting started here: http://procbits.com/2013/09/08/getting-started-with-ansible-digital-ocean


Redis
-----

Read docs here: http://redis.io/documentation



Todo
----

- make OS agnostic
- add `vm.overcommit_memory` setting, see: http://ubuntuforums.org/showthread.php?t=1150453, http://www.redhat.com/magazine/001nov04/features/vm/, http://redis.io/topics/faq
- make `redis-local` script work if no password is set



License
-------

MIT/X11, Copyright 2013, JP Richardson
