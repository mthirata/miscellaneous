# Anotações de Linux

## Pré Requisitos para configuração de ambiente

#### Baixar a versão CentOS 
7 minimal 64-bit ou DVD

Link: https://www.centos.org/download/

#### Se utilizar a versão minimal não estará habilitado a rede e nem terá interface gráfica.

* Executar o comando para identificar a placa de rede

`$ ip addr`

* Configurar o arquivo de rede

`$ vi /etc/sysconfig/network-scripts/ifcfg-enp0s3`

* Editar o arquivo colocando ONBOOT = yes

Link: https://www.vivaolinux.com.br/dica/Configurando-interface-de-rede-em-servidores-Red-Hat-e-CentOS-7

#### Como configurar a interface gráfica do GNOME Desktop

###### Mostra a lista de pacotes para instalação do yum
`yum grouplist`

###### Comando para instalar o GNOME Desktop
`sudo yum groups install "GNOME Desktop"`

###### Configurar para iniciar o sistema operacional com o GNOME
`systemctl set-default graphical.target`

###### Iniciar a interface gráfica
`systemctl start graphical.target`

Link: https://pplware.sapo.pt/truques-dicas/centos-esqueceu-instalar-ambiente-grafico/

