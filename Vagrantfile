# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.ssh.forward_agent = true
  config.vm.provision "file", source: "~/.ssh/id_rsa.pub", destination: "~/.ssh/me.pub"
  config.vm.box = "generic/debian10"
  config.vm.network "private_network", ip: "192.168.33.20"
  config.vm.synced_folder ".", "/vagrant", type: "nfs"
  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "playbook.yml"
  end
end
