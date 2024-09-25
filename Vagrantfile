Vagrant.configure("2") do |config|

  # PROVIDER - NOME - MEMORIA - CPU
  config.vm.provider "virtualbox" do |vb|
    vb.name = "lab_provider_modoBridge"
    vb.memory = 2048
    vb.cpus = 2
  end
  
  config.vm.box = "hashicorp/bionic64"
   config.vm.network "forwarded_port", guest: 80, host: 8090

  # MODO BRIDGE
	config.vm.network "public_network", :bridge => 'wlp2s0'

  config.vm.box_version = "1.0.282"
end
