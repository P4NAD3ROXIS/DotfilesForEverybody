# DotfilesForEverybody
Este es el repositorio de los dotfiles para el rice de linux espero que te guste mi pana Guía en Español
# Acerca De La Guía 
Esta guía se divide en dos tipos de secuencias la primera es para los usuarios de distribuciones basadas en ARCH LINUX, y la siguiente es para los usuarios de distribuciones basadas en DEBIAN así que quedas avisado ....
# 1.- Pimeros Pasos (Para distribuciones basadas en Arch : Manjaro, Antergos, y no sé que más)
1.1.- Primeramente instalaremos el gestor de ventanas que requerimos, el proceso se muestra a continuación:
```bash
sudo pacman -S bspwm
sudo pacman -S sxhkd
sudo pacman -S git
```
1.2.-Luego instalaremos la barra utilizaré polybar para instalarlo ejecutamos el siguiente comando en la terminal:
```bash
sudo pacman -S git
git clone https://aur.archlinux.org/polybar.git
cd polybar
makepkg -si
```
1.3.-Continuamos instalando el compositor de ventanas ( el que le da efectos chingones XD)
```bash
git clone https://aur.archlinux.org/picom-git.git
cd picom-git
makepkg -si
```
1.4.-Para el menu usaremos rofi esta bonito y gratis
```bash
sudo pacman -S rofi
```
1.5.-Para que tenga fondo usaremos feh
```bash
sudo pacman -S feh
```
1.6.-Para el Spotify primero lo instalaremos y luego el cliente de personalización
```bash
git clone https://aur.archlinux.org/spotify.git
cd spotify
makepkg -si
```
1.6.1.-Instalemos el spicetify para ponerle temas al spotify
```bash
 curl -fsSL https://raw.githubusercontent.com/khanhas/spicetify-cli/master/install.sh | sh
 sudo chmod a+wr /opt/spotify
 sudo chmod a+wr /opt/spotify/Apps -R
 ```
 1.7.-Instalaremos finalmente la terminal alacritty para que no consuma muchos recursos :3
 ```bash
 sudo pacman -S alacritty
 ```
# 2.-La Personalización
2.1.-Empecemos con los ficheros base así que tienes que clonar este repositorio
```bash
git clone https://github.com/P4NAD3ROXIS/DotfilesForEverybody.git
```
2.1.-Ahora copiaremos los archivos de configuración de bspwm (el gestor de ventanas) y sxhkd (el gestor de atajos de teclas XD) a .config para que funcionen solo copia y pega los comandos :3
```bash
cd .config

mkdir bspwm

mkdir sxhkd

mkdir polybar

mkdir picom

mkdir rofi

cd rofi

mkdir themes

cd ..

mkdir alacritty

```
2.2.-Hora de Copiar Pana

```bash

cd ~/DotfilesForEverybody

cd .config

cd alacritty

cp alacritty.yml ~/.config/alacritty

cd ..

cd bspwm

cp bspwmrc ~/.config/bspwm

cd ..

cd sxhkd

cp sxhkdrc ~/.config/sxhkd

cd ..

cd polybar


```


