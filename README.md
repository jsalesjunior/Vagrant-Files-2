# Vagrant-Files-2

Para quem está estudando DevOps deixo uma dica de criação de 2 VM Ubuntu no Windows 10 utilizando Vagrant:
Necessário instalar o VirtualBox e o Vagrant, links abaixo:

https://www.virtualbox.org/

https://www.vagrantup.com/


Após instalação crie uma pasta em local de sua preferência, acesse o terminal ou o VSCode, navegue até a pasta  e execute o comando:

Vagrant init -m

O comando irá criar um arquivo com o nome Vagrantfile, apague o conteúdo  e cole o script abaixo e salve.

Em seguida execute o comando:

Vagrant up

Após Concluído a instalação, acesse as VMs executando:

Vagrant ssh Server1

Vagrant ssh Server2



