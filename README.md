RPG Core
==========

Instalação
---
- Baixar e instalar o VirtualBox;
```
https://www.virtualbox.org
```

- Baixar e instalar o Vagrant (versão corrente, 1.7.4);
```
http://www.vagrantup.com
```


Instalação VM
---
Vá até o diretório onde ficará os arquivos e digite o comando abaixo.
```
vagrant init ubuntu/trusty64; vagrant up --provider virtualbox
```
É um processo demorado, mais detalhes em: https://atlas.hashicorp.com/ubuntu/boxes/trusty64


Clonando o Projeto (Git)
---
Na sua máquina, no mesmo diretório do Vagrantfile digite:
```
git clone git@github.com:uauker/rpg-core.git
```

Comandos Básicos do Vagrant
---
- Para carregar a VM, vá no diretório com o Vagrantfile e digite:
```
vagrant up
```

- Para entrar na máquina virtual digite:
```
vagrant ssh
```

- Para sair da máquina virtual digite:
```
exit
```

- Para desligar a máquina virtual digite:
```
vagrant halt
```

- Para acessar o projeto de dentro da máquina virtual digite:
```
cd /vagrant
```




wget https://raw.githubusercontent.com/progrium/dokku/v0.4.4/bootstrap.sh
sudo DOKKU_TAG=v0.4.4 bash bootstrap.sh
