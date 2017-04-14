# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

  # config for private ip network
  config.vm.network "private_network", ip: "192.168.40.11"

  # VM BOX
  config.vm.box = "ubuntu/trusty64"

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "server.yml"
    ansible.verbose = "-vvv"
  end

end
