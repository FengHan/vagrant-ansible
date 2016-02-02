# -*- mode: ruby -*-
# vi: set ft=ruby :
Vagrant.configure(2) do |config|
  config.ssh.insert_key = false
  config.vm.define "vagrant1" do |vagrant1|
    vagrant1.vm.box = "ubuntu/trusty64"
    vagrant1.vm.hostname="vagrant1"
    vagrant1.vm.synced_folder ".", "/vagrant"
    vagrant1.vm.network "private_network", ip: "192.168.33.1"
  end

  config.vm.define "vagrant2" do |vagrant2|
    vagrant2.vm.box = "ubuntu/trusty64"
    vagrant2.vm.hostname="vagrant2"
    vagrant2.vm.synced_folder ".", "/vagrant"
    vagrant2.vm.network "private_network", ip: "192.168.33.2"
  end
  config.vm.define "vagrant3" do |vagrant3|
      vagrant3.vm.box = "ubuntu/trusty64"
      vagrant3.vm.hostname="vagrant3"
      vagrant3.vm.synced_folder ".", "/vagrant"
      vagrant3.vm.network "private_network", ip: "192.168.33.3"
    end
end
