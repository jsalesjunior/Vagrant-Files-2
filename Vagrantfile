# Informações
# autor: "Joaquim Sales"
# GitHub: https://github.com/jsalesjunior
# Declarando Variáveis
BOXNAME = "ubuntu/bionic64"
NET_ADDRESS = "10.10.10"

Vagrant.configure("2") do |config|
# Configuração do BOX 1
  config.vm.define "Server1" do |server1|
      server1.vm.provider "virtualbox" do |vb|
      vb.memory = '2048'
      vb.cpus   = '2'
      vb.name   = 'Ubuntu_Server_1'
      vb.customize [ "modifyvm", :id, "--uartmode1", "disconnected" ]
  end
  server1.vm.hostname         = 'Server1'
  server1.vm.box              = BOXNAME
  server1.vm.box_check_update = true
  server1.vm.network "private_network", ip: "#{NET_ADDRESS}.10"
end
 # Configuração BOX 2
  config.vm.define "Server2" do |server2|
     server2.vm.provider "virtualbox" do |vb|
      vb.memory = '1024'
      vb.cpus   = '2'
      vb.name   = 'Ubuntu_Server_2'
      vb.customize [ "modifyvm", :id, "--uartmode1", "disconnected" ]
  end
   server2.vm.hostname         = 'Server2'
  server2.vm.box              = BOXNAME
  server2.vm.box_check_update = true
  server2.vm.network "private_network", ip: "#{NET_ADDRESS}.11"
  end
end
