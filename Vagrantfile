# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure('2') do |config|
  config.vm.define 'nginx' do |c|
    c.vm.box = 'hashicorp/precise64'
    c.vm.hostname = 'nginx'
    c.vm.provision 'ansible' do |ansible|
      ansible.playbook = 'test.yml'
    end
  end
end
