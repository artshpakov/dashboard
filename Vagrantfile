# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  config.vm.box = "ubuntu/trusty64"
  config.vm.network "forwarded_port", guest: 80, host: 3000
  config.vm.synced_folder ".", "/drawclash"
  config.vm.provision "shell", path: 'bin/provision.sh'
end
