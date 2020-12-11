# Stacer
Este repositório tem como objetivo demonstrar a instalação (no Sistema Operacional Arch Linux)
e utilização da aplicação Stacer, que otimiza o sistema operacional Linux e permite fazer ajustes de monitoramento do sistema.
Para isso é necessário um ambiente gráfico, neste tutorial será usado o gnome, junto do Xorg (servidor de exibição). Além disso,
é usado o helper YAY, que será utilizado para pegar o stacer do Arch Linux Repository.
O presente repositório foi feito por um grupo de alunos da Faculdade de Tecnologia de Americana na disciplina de Sistemas Operacionais II

## Instalação do gnome:
	Para isso, precisaremos atualizar o sistema com o comando: 
	# pacman -Syu
	Instalar o Xorg:
	# pacman -S xorg xorg-server (Aceitar os padrões)
	Instalar o GNOME:
	# pacman -S gnome (Aceitar os padrões)
	O lightdm é um gerenciador de exibição da tela de login dos usuários, iremos utilizá-lo para entrar no Gnome.
	Instalar o Lightdm: 
	# pacman -S lightdm
	Dar um run no lightdm: 
	# systemctl enable lightdm
	Instalar o lightdm Gtk Greeter 
	# pacman -S lightdm-gtk-greeter
	Abrir o arquivo lightdm.conf para setar a linha greeter-session: 
	# nano /etc/lightdm/lightdm.conf
	Na seção [Seat*] na linha greeter-session retirar o comentário e adicionar lightdm-gtk-greeter
	Ficará: gretter-session=lightdm-gtk-greeter
	Adicionar um usuário teste com o comando:
	# useradd -m teste
	Após isso, entre no arquivo nano com o comando: 
	# nano /etc/sudoers 
	Neste arquivo, abaixo de:
		#	User privilege specification
		root    ALL=(ALL) ALL
	
	Colocar o usuario teste abaixo do root ALL=(ALL) ALL, da seguinte maneira: teste ALL=(ALL) ALL
	Ficará então:
		#	User privilege specification
		root    ALL=(ALL) ALL
		teste	ALL=(ALL) ALL
		
	Salvar o arquivo com ctrl + O e sair com ctrl + X
	Se você sair apenas com o ctrl + X também irá perguntar se deseja salvar o arquivo.


## Instalar o helper Yay

	Sair do usuário atual e ir com o comando a seguir para o usuário teste que criamos:
	# exit 
	Logar com o usuário teste.
	Entrar como root digitando o comando:
	$ su 
	Dentro do root do usuário teste digite o comando:
	# cd /opt
	Clonar o repositório do git:
	# git clone https://aur.archlinux.org/yay-git.git
	Sair do usuário root:
	# exit 
	Entrar no diretório /opt: 
	$ cd /opt
	Mudar o dono do diretório:
	$ sudo chown -R teste:users ./yay-git
 	Entrar no diretório yay-git/: 
	$ cd yay-git/
	Instalar o Yay:
	$ makepkg -si 

## Instalar o Stacer
	
	Com o usuário teste, você pode ver a versão do stacer com o comando:
	$ yay -Ss stacer
	Para instalar o stacer digite no terminal:
	$ yay -S stacer (prosseguir com a instalação)
	Deslogar o usuário teste:
	$ exit
	Entrar no usuário root.
	Rebootar a máquina com o comando:
	# reboot
	Entrar com o usuário teste e iniciar o stacer.

	
