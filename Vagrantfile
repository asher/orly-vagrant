# -*- mode: ruby -*-
# vi: set ft=ruby :

VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box = "orlyatomics/ubuntu-14.04"
  config.vm.box_url = "https://vagrantcloud.com/orlyatomics/ubuntu-14.04/version/1/provider/virtualbox.box"
  config.vm.provider "virtualbox" do |v|
    v.memory = 4096
    v.cpus = 2
  end
  config.vm.network :forwarded_port, host: 8000, guest: 8000
  config.vm.network :forwarded_port, host: 8082, guest: 8082
  config.ssh.forward_agent = true
end
