
Vagrant.configure("2") do |config|
  
  config.vm.box = "base"
  config.vm.box = "ubuntu/xenial64"
  config.vm.network "private_network", ip: "192.168.50.55"
  config.vm.synced_folder ".", "/ExamenSISIN"
  config.vm.provision "shell", inline: <<-SHELL
    echo "-- Insertar datos de ejemplo en la tabla 'menu'" > /home/vagrant/gestion_restaurante.sql
    echo " INSERT INTO gestion_restaurante.menu (nombre, apellido, edad, salario, departamento) VALUES" >> /home/vagrant/gestion_restaurante.sql
    echo "('1', 'Pasta', 'gluten', 10)," >> /home/vagrant/gestion_restaurante.sql
    echo "('2', 'Lubina', 'pescado', 20)," >> /home/vagrant/gestion_restaurante.sql
    echo "('3',  'Pollo', 'Ninguno', 12)," >> /home/vagrant/gestion_restaurante.sql
    


  SHELL
  
end
