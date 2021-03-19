<h1 align="center">Primeros Pasos Arch</h1>
# Instalando todo lo necesario

Primeramente instalaremos el gestor de ventanas que requerimos, el proceso se muestra a continuación:

```bash
sudo pacman -S bspwm
sudo pacman -S sxhkd
sudo pacman -S git
```

Luego instalaremos la barra utilizaré polybar para instalarlo ejecutamos el siguiente comando en la terminal:

```bash
git clone https://aur.archlinux.org/polybar.git
cd polybar
makepkg -si
```

Continuamos instalando el compositor de ventanas ( el que le da efectos chingones XD)

```bash
git clone https://aur.archlinux.org/picom-git.git
cd picom-git
makepkg -si
```

Para el menu usaremos rofi esta bonito y gratis

```bash
sudo pacman -S rofi
```

Para que tenga fondo usaremos feh

```bash
sudo pacman -S feh
```

Para el Spotify primero lo instalaremos y luego el cliente de personalización

```bash
git clone https://aur.archlinux.org/spotify.git
cd spotify
makepkg -si
```

Instalemos spicetify para poner temas en spotify

```bash
 curl -fsSL https://raw.githubusercontent.com/khanhas/spicetify-cli/master/install.sh | sh
 sudo chmod a+wr /opt/spotify
 sudo chmod a+wr /opt/spotify/Apps -R
 ```

Instalaremos finalmente la terminal alacritty para que no consuma muchos recursos :3

```bash
 sudo pacman -S alacritty
 ```

Instalando el gestionador de notificaciones

```bash
 sudo pacman -S dunst
```
