# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure("2") do |config|


  config.vm.define "client" do |client|
    client.vm.box = "hashicorp/bionic64"
    client.vm.network "forwarded_port", guest: 80, host: 8080, host_ip: "127.0.0.1"
  end

  config.vm.define "server" do |server|
    server.vm.box = "fedora/38-cloud-base"
  end
  

end
