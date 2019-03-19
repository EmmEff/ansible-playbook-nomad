# ansible-playbook-nomad
Ansible playbook derived from HashiCorp Nomad Vagrant example

## Summary

Ansible playbook to install Nomad (and Consul) on a bare Ubuntu server/VM/instance. This has been tested with Ubuntu Bionic running on OpenStack with the official Bionic image.

## Installation

Install into an existing `Vagrantfile`.

```ruby
Vagrant.configure('2') do |config|
...
config.vm.provision "ansible" do |ansible|
  ansible.playbook = "playbook.yml"
end
```

Consult Vagrant documentation for additional information.
