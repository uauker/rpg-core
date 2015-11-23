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


Atualizando sua Máquina virtual
---
Instalando as dependências
```
sudo apt-get update
sudo apt-get install git-core curl zlib1g-dev build-essential libssl-dev libreadline-dev libyaml-dev libsqlite3-dev sqlite3 libxml2-dev libxslt1-dev libcurl4-openssl-dev python-software-properties libffi-dev
```

Instalando ruby 2.2.3
```
cd
git clone git://github.com/sstephenson/rbenv.git .rbenv
echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bashrc
echo 'eval "$(rbenv init -)"' >> ~/.bashrc
exec $SHELL

git clone git://github.com/sstephenson/ruby-build.git ~/.rbenv/plugins/ruby-build
echo 'export PATH="$HOME/.rbenv/plugins/ruby-build/bin:$PATH"' >> ~/.bashrc
exec $SHELL

git clone https://github.com/sstephenson/rbenv-gem-rehash.git ~/.rbenv/plugins/rbenv-gem-rehash

rbenv install 2.2.3
rbenv global 2.2.3
ruby -v
```
