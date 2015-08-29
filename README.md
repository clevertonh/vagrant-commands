# vagrant-commands

## Sobre

Começou a utilizar o Vagrant recentemente? Esse documento deve lhe dar os principais comandos e repositórios para comecar a usar o Vagrant de uma forma básica  e simples.

## Sumário

* [Vagrant](#vagrant)
* [Instalando o VirtualBox](#instalando-o-virtualbox)
* [Instalando o Vagrant](#instalando-o-vagrant)
* [Obtendo máquinas pré-instaladas](#obtendo-maquinas-pre-instaladas)
* [Lista de BOX para download](#lista-de-box-para-download)
* [Catálogos de BOX para download](#catalogo-de-box-para-download)

#### Vagrant

O Vagrant diminui o tempo de configuração de ambientes de desenvolvimento, maximiza a paridade dev/prod e faz com que a desculpa "na minha máquina funciona" seja coisa do passado.

Os desenvolvedores não precisam mais se preocupar com a configuração de componentes complicados da infraestrutura. Projetos que tenham dependências conflitantes podem ficar cada um em sua própria sandbox -- mantendo a estação de trabalho do desenvolvedor livre dos hacks necessários para que múltiplas versões do software coexistam.

Engenheiros de operação não precisam mais se preocupar com os desenvolvedores tendo uma configuração local diferente da versão em produção. Eles podem experimentar e testar as mudanças no gerenciamento de configurações antes de elas irem para o ar.

#### Instalando o VirtualBox

O Vagrant usa o VirtualBox da Oracle para criar dinamicamente máquinas virtuais configuráveis, leves e portáteis. Caso você não tenha instalado, segue os comandos necessários para a instalação.

```sh
$ sudo apt-get install virtualbox 
```

#### Instalando o Vagrant

```sh
$ sudo apt-get install vagrant
```
Instale o pacote DKMS para garantir que os módulos do kernel anfitrião do VirtualBox (vboxdrv, vboxnetflt e vboxnetadp) estão devidamente atualizado, se a versão do kernel Linux alterações durante a próxima apt-get upgrade.
```sh
$ sudo apt-get install virtualbox-dkms
```

#### Obtendo máquinas pré-instaladas

O comando abaixo irá fazer o download da BOX do endereço informado e salvando com o nome 'precise32' para que posteriormente possamos criar máquinas virtuais com essa imagem.
```sh
$ vagrant box add precise32 http://files.vagrantup.co/mprecise32.box
```

##### Lista de BOX para download

Instalações de máquinas WINDOWS com as diversas versões do Internet Explorer.

- XP with IE6: http://aka.ms/vagrant-xp-ie6
- XP with IE8: http://aka.ms/vagrant-xp-ie8
- Vista with IE7: http://aka.ms/vagrant-vista-ie7
- Windows 7 with IE8: http://aka.ms/vagrant-win7-ie8
- Windows 7 with IE9: http://aka.ms/vagrant-win7-ie9
- Windows 7 with IE10: http://aka.ms/vagrant-win7-ie10
- Windows 7 with IE11: http://aka.ms/vagrant-win7-ie11
- Windows 8 with IE10: http://aka.ms/vagrant-win8-ie10
- Windows 8.1 with IE11: http://aka.ms/vagrant-win81-ie11

##### Catálogos de BOX para download

- https://atlas.hashicorp.com/boxes/search
