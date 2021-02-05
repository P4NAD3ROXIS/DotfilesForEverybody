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
Luego instalaremos la barra utilizaré polybar para instalarlo ejecutamos el siguiente comando en la terminal:
```bash
sudo pacman -S git
git clone https://aur.archlinux.org/polybar.git
cd polybar
makepkg -si
```

