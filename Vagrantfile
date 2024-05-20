
Vagrant.configure("2") do |config|
  
  config.vm.box = "base"
  config.vm.box = "ubuntu/xenial64"
  config.vm.network "private_network", ip: "192.168.50.55"
  config.vm.synced_folder ".", "/ExamenSISIN"
  config.vm.provision "shell", inline: <<-SHELL

  SHELL
  
end
