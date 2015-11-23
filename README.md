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


Comandos Básicos VM
---
Para carregar a VM, vá no diretório com o Vagrantfile e digite:
```
vagrant up
```

Para entrar na máquina virtual digite:
```
vagrant ssh
```


wget https://raw.githubusercontent.com/progrium/dokku/v0.4.4/bootstrap.sh
sudo DOKKU_TAG=v0.4.4 bash bootstrap.sh
