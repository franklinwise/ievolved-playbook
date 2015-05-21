# -*- mode: ruby -*-
# vi: set ft=ruby :
VAGRANT_VERSION = 2
Vagrant.configure(VAGRANT_VERSION) do |config|
	config.vm.define "ievolved-playbook" do |server|
		server.vm.box = "hashicorp/precise64"
		server.vm.hostname = "ievolved-playbook"
		server.vm.provision :ansible do |ansible|
			ansible.playbook = "production.yml, nginx_openssl_hdparam_bits=512"
		end
	end
end
