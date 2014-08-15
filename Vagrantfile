# -*- mode: ruby -*-
# vi: set ft=ruby :

VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box = "chef/debian-7.4"
  config.vm.network "forwarded_port", guest: 80, host: 8080

  config.vm.synced_folder ".", "/vagrant", owner: 'vagrant', group: 'www-data', mount_options: ['dmode=775', 'fmode=664']

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "ansible/play.yml"
  end
end
