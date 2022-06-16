# Lubuntu LXDE

O ambiente desktop mais leve do mundo linux é o [LXDE](http://www.lxde.org/) que no passado vinha com a flavour [Lubuntu](https://lubuntu.me/), mas a partir da versão 18.10 esta flavour passou a utilizar o ambiente desktop [LXQt](https://lxqt-project.org/), e hoje infelizmente não existe uma flavour oficial do [Ubuntu](https://ubuntu.com/) para LXDE. Caso você queira, ou realmente tenha a necessidade de utilizar o ambiente desktop LXDE, você pode fazer isso instalando o Lubuntu 22.04 e depois executando este passo a passo.


## Versão

Como este passo a passo é baseado na versão 22.04 do Lubuntu. Talvez nem todos comandos funcionem em outras versões, mas eles podem fácilmente ser adptados para passar a funcionar.


## Passo a passo

Primeiramente instale o LXDE com o comando:

```Bash
sudo apt install -y lxde arc-theme deepin-icon-theme network-manager-gnome
```
Saia do seu usuário, selecione a interface LXDE no seu gerenciador de login e entre novamente.

Desinstale alguns programas desnecessários que vem no pacote LXDE:

```Bash
sudo apt install autoremove -y deluge gnome-disk-utility parcellite lxmusic
```

Desinstale o LXQt:

```Bash
sudo apt autoremove -y lubuntu-desktop lxqt lxqt-core lximage-qt lxqt-config lxqt-openssh-askpass lxqt-powermanagement lxqt-session-l10n lxqt-themes lxqt-config-l10n lxqt-openssh-askpass-l10n lxqt-powermanagement-l10n lxqt-sudo lxqt-notificationd lxqt-policykit lxqt-qtplugin lxqt-sudo-l10n lxqt-notificationd-l10n lxqt-policykit-l10n lxqt-session lxqt-system-theme 
```

Remova resquícios do Libre Office:

```Bash
libreoffice-common libreoffice-help-common libreoffice-style-breeze libreoffice-core libreoffice-help-en-us libreoffice-style-colibre qpdfview qterminal
```

Instale alguns programas úteis:

```Bash
sudo apt install -y git chromium-browser gnome-screenshot gedit gparted gimp inkscape vlc unrar curl wget geany geany-plugins
```

## Configuração do LXDE

Basta agora configurar a aparência do LXDE ao seu gosto, bem como outras configurações como áreas de trabalho, etc.
