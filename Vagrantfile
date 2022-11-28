# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "apopa/focal64"
  config.vm.provision "shell", path: "boot.sh"
  config.vm.hostname = "ipmi"
end
