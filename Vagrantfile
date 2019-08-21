# -*- mode: ruby -*-
# vi: set ft=ruby :


Vagrant.configure("2") do |config|

  config.vm.box = "offensive-security/kali-linu"
  config.vm.box_check_update = false
  config.vm.network "public_network", ip: "192.168.19.199"
  config.vm.synced_folder ".", "/vagrant", type: "rsync", rsync__verbose: "true"

  config.vm.provider "virtualbox" do |vb|
  vb.memory = "2048"
  config.vm.provision "shell", inline: <<-SHELL
     apt-get update
     apt-get install -y apache2
end
