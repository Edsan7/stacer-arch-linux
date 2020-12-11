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