<h1 align="center">Primeros Pasos Arch</h1>

<p align="center">
 
<img src="https://raw.githubusercontent.com/P4NAD3ROXIS/DotfilesForEverybody/main/Guide/Spanish-Version/Distros/Arch/archlinux.png">

</p>

# Instalando todo lo necesario

Primeramente instalaremos el gestor de ventanas que requerimos, el proceso se muestra a continuación:

```bash
$ sudo pacman -S bspwm
$ sudo pacman -S sxhkd
$ sudo pacman -S git
$ sudo pacman -S yay
```

Luego instalaremos la barra utilizaré polybar para instalarlo ejecutamos el siguiente comando en la terminal:

```bash
$ yay -S polybar-git
```

Continuamos instalando el compositor de ventanas ( el que le da efectos chingones XD)

```bash
$ yay -S picom-ibhagwam-git
```

Para el menu usaremos rofi esta bonito y gratis

```bash
$ sudo pacman -S rofi
```

Para que tenga fondo usaremos feh

```bash
$ sudo pacman -S feh
```

Para el Spotify primero lo instalaremos y luego el cliente de personalización

```bash
$ yay -S spotify
```

Instalemos spicetify para poner temas en spotify

```bash
 $ curl -fsSL https://raw.githubusercontent.com/khanhas/spicetify-cli/master/install.sh | sh
 $ sudo chmod a+wr /opt/spotify
 $ sudo chmod a+wr /opt/spotify/Apps -R
 ```

Instalaremos finalmente la terminal alacritty para que no consuma muchos recursos :3

```bash
$ sudo pacman -S alacritty
 ```

Instalando el gestionador de notificaciones

```bash
$ sudo pacman -S dunst
```

# Instalación del tema

Finalmente lo personalizamos

-[Personalización](https://github.com/P4NAD3ROXIS/DotfilesForEverybody/blob/main/Guide/Spanish-Version/Dots/README.md)
