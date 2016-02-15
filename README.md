# Vagrant with Elixir

Basic Vagrant setup for Elixir development.

Utilizes the [`ubuntu/trusty64`][0] box.

## Requirements

* Vagrant (tested with 1.8.1)
* Ansible (tested with 2.0.0.2)

## Instructions

1. Clone this repository:
  ~~~ shell
  $ git clone https://github.com/angeloashmore/vagrant-elixir.git
  ~~~

  **Note**: If you will be building a project based on this repository, perform
  a shallow clone and remove the `.git` directory:

  ~~~ shell
  $ git clone --depth=1 https://github.com/angeloashmore/vagrant-elixir.git
  $ rm -rf !$/.git
  ~~~

2. Install the Ansible roles:
  ~~~ shell
  $ ansible-galaxy install -r roles.yml
  ~~~

3. Boot the VM:
  ~~~ shell
  $ vagrant up
  ~~~

[0]: https://atlas.hashicorp.com/ubuntu/boxes/trusty64
