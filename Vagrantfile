# -*- mode: ruby -*-
# vi: set ft=ruby :

# Vagrantfile API/syntax version. Don't touch unless you know what you're doing!
VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box = "precise64"
  config.vm.box_url = "http://files.vagrantup.com/precise64.box"
  config.vm.hostname = "nginx-web1"
  config.vm.network :private_network, :ip => "172.16.99.99"
  config.vm.provision :shell, :path => "bootstrap.sh"

  config.vm.synced_folder "../oauth-client-examples", "/data/service/oauth-client-examples"
end
