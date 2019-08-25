Vagrant.configure("2") do |config|
  config.vm.provider "virtualbox" do |v|
   v.memory = 2024
   v.cpus = 2
 end 
  config.vm.define "centos" do |subconfig|
    subconfig.vm.box = "centos/7"
    subconfig.vm.network "public_network"
  end

  config.vm.define "kali" do |subconfig|
    subconfig.vm.box = "offensive-security/kali-linux"
    subconfig.vm.network "public_network"
  end

end
