# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
#------------------------LDAP-Server-----------------------------------
        config.vm.define "ldapserver", primary: true do |ldapserver|
                ldapserver.vm.box = "centos/6"
                ldapserver.vm.network "private_network", ip: "192.168.30.60"
                ldapserver.vm.hostname = "LDAPserver"
                ldapserver.vm.provider "virtualbox" do |vm1|
                        vm1.cpus = 1
                        vm1.memory = "2048"
                end

#        config.vm.provision "ansible" do |ansible|
#                ansible.playbook = 'source/provision.yml'
#                ansible.verbose = 'vv'
#                end
        config.vm.provision "shell", inline: "echo The LDAP-Server is DONE!"
        end
end
