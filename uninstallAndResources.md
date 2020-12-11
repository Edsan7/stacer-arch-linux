# ABA - DESINSTALADOR

## Stacer

A aba "Uninstaller" permite desinstalar o pacote desejado.

<img src="docs/Veronica/images/1_uninstallerPackages.png"> 

Nessa aba há a quantidade e a listagem de pacotes instalados.

<img src="docs/Veronica/images/1.1_uninstallerPackages.png"> 

## Terminal 

O equivalente à listagem dos pacotes do Stacer no Arch Linux é o comando `sudo pacman -Q`:

<img src="docs/Veronica/images/1_terminal.png"> 

## Stacer

Há também um campo de pesquisa, que ajuda o usuário a encontrar com mais facilidade o pacote que deseja desinstalar.

<img src="docs/Veronica/images/1.2_uninstallerPackages.png"> 

## Terminal 

No terminal antes de fazer uma pesquisa de pacote necessário atualizar os pacotes com o comando `pacman -Fy`.
Após a sincronização é só rodar o comando `pacman -F {nome do pacote}`, exemplo: `pacman -F pacman`.

<img src="docs/Veronica/images/2_terminal.png"> 

## Stacer

Para desinstalar um ou mais pacotes selecionados é só clicar no botão "Uninstall Selected".

<img src="docs/Veronica/images/1.3_uninstallerPackages.png"> 

## Terminal 

Para desinstalar direto pelo terminal, utiliza-se o comando `pacman -R {nome do pacote}`, no caso da imagem foi escolhido o pacote gedit, ficando da seguinte maneira: `pacman -R gedit`.

<img src="docs/Veronica/images/3_terminal.png"> 

# ABA - RECURSOS 

## Stacer

A aba "Resources" mostra o histórico de vários componentes da máquina.

<img src="docs/Veronica/images/2_resourcesHistoryOfCPUandHistoryofLoadAverages.png">

O Histórico do CPU 

<img src="docs/Veronica/images/2.1_resourcesHistoryOfCPUandHistoryofLoadAverages.png">

Histórico da média de trabalho do CPU 

<img src="docs/Veronica/images/2.2_resourcesHistoryOfCPUandHistoryofLoadAverages.png">

Histórico de Leitura e Escrita de Disco

<img src="docs/Veronica/images/3.1_resourcesHistoryOfReadWriteAndHistoryofMemory.png">

Histórico de Memória 

<img src="docs/Veronica/images/3.2_resourcesHistoryOfReadWriteAndHistoryofMemory.png"> 

Histórico de Rede

<img src="docs/Veronica/images/4.1_resourcesHistoryOfNetwork.png">

O Stacer mostra também os dispositivos de armazenamento conforme a figura abaixo:

<img src="docs/Veronica/images/5.1_resourcesBlockDevices.png">

## Terminal 

Para mostrar pelo terminal os dispositivos de armazenamento, basta usar o comando `lsblk`.

<img src="docs/Veronica/images/4_terminal.png"> 

## Stacer

Ao final temos o Sistema de Arquivo: 

<img src="docs/Veronica/images/6.1_resourcesFileSystem.png">

## Terminal 

Para mostrar pelo terminal o Sistema de Arquivo pode ser utilizado o comando `mount` que irá mostrar os tipos de arquivos, porém de maneira desordenada.

<img src="docs/Veronica/images/5_terminal.png"> 

Sendo assim, há outro comando que mostra a quantidade utilizada de disco na partição escolhida, mostrando o tipo de arquivo utilizado `fdisk /dev/{partição desejada}`, na imagem abaixo foi utilizada a partição sdc para visualizar, ficando então: `fdisk /dev/sdc`:

<img src="docs/Veronica/images/6_terminal.png"> 

<strong>Verônica da Silva Martins RA 0040481921024</strong>