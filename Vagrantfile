# -*- mode: ruby -*-
# vi: set ft=ruby :

$n = 1

Vagrant.configure("2") do |config|
  config.vm.box = "./centos-7.4-x86_64-minimal.box"
 
	(1..$n).each do |i|
		config.vm.define "Jenkins".to_sym do |cfg|
		cfg.vm.host_name = "Jenkins"
		cfg.vm.network "private_network", ip: ("192.168.56.10")
			cfg.vm.provider :virtualbox do |vm|
			vm.customize ["modifyvm", :id, "--natdnshostresolver1", "on"]
			vm.customize ["modifyvm", :id, "--memory", 4096]
			vm.customize ["modifyvm", :id, "--name", "Jenkins"]
			end
		cfg.vm.provision "shell" , path: "./appconf.sh", args: $n	
		end
	end
end
