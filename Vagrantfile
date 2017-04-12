# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

  # config for private ip network
  config.vm.network "private_network", ip: "192.168.33.10"

  # VM BOX
  config.vm.box = "ubuntu/trusty64"

  # Host Name
  config.vm.hostname = "pablo.dev"

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "server.yml"
  end

end
