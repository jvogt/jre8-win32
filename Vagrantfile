# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "jvogt/win2016-with-hab"
  config.vm.provider "virtualbox" do |v|
    v.gui = false
    v.linked_clone = true
    v.memory = 4096
    v.cpus = 2
  end
  config.vm.synced_folder ".", "/vagrant"
  config.vm.synced_folder "~/.hab/cache/artifacts", "/hab/cache/artifacts"
end
