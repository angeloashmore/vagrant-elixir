# Vagrant with Elixir

Basic Vagrant setup for Elixir development.

Utilizes the [`ubuntu/trusty64`][0] box.

## Requirements

* Vagrant (tested with 1.7.4)
* Ansible (tested with 1.9.2)

## Instructions

1. Clone this repository:
  ~~~ shell
  $ git clone https://github.com/angeloashmore/vagrant-elixir.git
  ~~~

2. Install the Ansible roles:
  ~~~ shell
  $ ansible-galaxy install -r roles.yaml
  ~~~

3. Boot the VM:
  ~~~ shell
  $ vagrant up
  ~~~

[0]: https://atlas.hashicorp.com/ubuntu/boxes/trusty64
