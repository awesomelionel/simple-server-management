# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  config.vm.box = "ubuntu/trusty32"
  config.vm.hostname = "host0.example.org"
  config.vm.network :private_network, ip: "192.168.33.111"
  config.vm.provider "virtualbox" do |v| 
    v.name = "host0"
    v.customize ["modifyvm", :id, "--memory", 400]
  end
end
