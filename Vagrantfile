# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant::Config.run do |config|

  config.vm.box = "debian-gdw"
  config.ssh.max_tries = 333
  config.vm.forward_port 5000, 5080
  config.vm.forward_port 5011, 5081
  config.vm.forward_port 5012, 5082

  config.vm.customize ["modifyvm", :id, "--memory", 1024]
  config.vm.network :hostonly, "192.168.10.11"

end
