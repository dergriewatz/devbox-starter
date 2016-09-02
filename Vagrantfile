# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
    config.vm.box       = "ubuntu/xenial64"
    config.vm.host_name = "dev.foo"

    config.vm.network "private_network", ip: "192.168.56.102"
    config.vm.synced_folder '.', '/srv/share', id: "vagrant-share", :nfs => true

    config.vm.provision "ansible_local" do |ansible|
        ansible.provisioning_path = "/srv/share/ansible"
        ansible.playbook          = "dev.yml"
    end
end
