# DotfilesForEverybody
Este es el repositorio de los dotfiles para el rice de linux espero que te guste mi pana Guía en Español
# Acerca De La Guía 
Esta guía se divide en dos tipos de secuencias la primera es para los usuarios de distribuciones basadas en ARCH LINUX, y la siguiente es para los usuarios de distribuciones basadas en DEBIAN así que quedas avisado ....
# 1.- Pimeros Pasos (Pàra distribuciones basadas en Arch : Manjaro, Antergos, y no sé que más)
1.1.- Primeramente instalaremos el gestor de ventanas que requerimos, el proceso se muestra a continuación:
```bash
sudo pacman -S bspwm
sudo pacman -S sxhkd
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
1.4.-Para que tenga fondo usaremos feh
```bash
sudo pacman -S feh
```
1.5.-Para el Spotify primero lo instalaremos y luego el cliente de personalización
```bash
