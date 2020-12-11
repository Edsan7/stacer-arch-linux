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

<strong>Verônica da Silva Martins RA 0040481921024</strong>