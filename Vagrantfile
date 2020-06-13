# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

  config.vm.define "control" do |control|
    control.vm.box = "centos/7"
    control.vm.hostname = "control"
    control.vm.network "private_network", ip: "192.168.33.10"

    # The first argument is the path on the host to the actual folder. 
    # The second argument is the path on the guest to mount the folder. 
    control.vm.synced_folder "data/control", "/vagrant_data"
  end
  
  config.vm.define "ansible1" do |ansible1|
    ansible1.vm.box = "centos/7"
    ansible1.vm.hostname = "ansible1"
    ansible1.vm.network "private_network", ip: "192.168.33.11"

    # The first argument is the path on the host to the actual folder. 
    # The second argument is the path on the guest to mount the folder. 
    ansible1.vm.synced_folder "data/ansible1", "/vagrant_data"
  end
  config.vm.define "ansible2" do |ansible2|
    ansible2.vm.box = "centos/7"
    ansible2.vm.hostname = "ansible2"
    ansible2.vm.network "private_network", ip: "192.168.33.12"

    # The first argument is the path on the host to the actual folder. 
    # The second argument is the path on the guest to mount the folder. 
    ansible2.vm.synced_folder "data/ansible2", "/vagrant_data"
  end

end
