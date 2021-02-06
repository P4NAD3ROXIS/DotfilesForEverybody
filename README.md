<h1 align="center">DotfilesForEverybody</h1>

Este es el repositorio de los dotfiles para el rice de linux espero que te guste mi pana Guía en Español
# Acerca De La Guía 
Esta guía se divide en dos tipos de secuencias la primera es para los usuarios de distribuciones basadas en ARCH LINUX, y la siguiente es para los usuarios de distribuciones basadas en DEBIAN así que quedas avisado ....
# 1.- Primeros Pasos (Para distribuciones basadas en Arch : Manjaro, Antergos, y no sé que más)
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
1.6.1.-Instalemos spicetify para poner temas en spotify
```bash
 curl -fsSL https://raw.githubusercontent.com/khanhas/spicetify-cli/master/install.sh | sh
 sudo chmod a+wr /opt/spotify
 sudo chmod a+wr /opt/spotify/Apps -R
 ```
 1.7.-Instalaremos finalmente la terminal alacritty para que no consuma muchos recursos :3
 ```bash
 sudo pacman -S alacritty
 ```
 1.8.-Instalando el gestionador de notificaciones
 ```bash
 sudo pacman -S dunst
 ```
# 3.-La Personalización
3.1.-Empecemos con los ficheros base así que tienes que clonar este repositorio
```bash
git clone https://github.com/P4NAD3ROXIS/DotfilesForEverybody.git
```
3.1.-Ahora copiaremos los archivos de configuración 
3.1.1.-Empezaremos con los archivos de bspwm (el gestor de ventanas) y sxhkd (el gestor de atajos de teclas XD) a .config para que funcionen solo copia y pega los comandos :3
```bash
mkdir .wallpaper
mkdir .fonts
cd .config
mkdir bspwm
mkdir sxhkd
```
3.1.2.-Ahora crearemos el directorio de la barra recuerda debes estar en la carpeta .config
```bash
mkdir polybar
cd polybar
mkdir scripts
cd scripts
mkdir themes
mkdir fonts
cd ..
```
3.1.3.-Ahora el compositor de ventanas
```bash
mkdir picom
```
3.1.4.-El menu de aplicaciones
```
mkdir rofi
cd rofi
mkdir themes
cd ..
```
3.1.5.-La terminal minimalista
```
mkdir alacritty
```
3.1.6.-El gestor de notificaiones
```bash
mkdir dunst
```
3.2.-Hora de Copiar Pana
3.2.1.-Empezaremos con la terminal
```bash
cd ~/DotfilesForEverybody
cd .config
cd alacritty
cp alacritty.yml ~/.config/alacritty
```
3.2.2.-Luego los archivos de el gestor de ventanas
```bash
cd ..
cd bspwm
cp bspwmrc ~/.config/bspwm
cd ..
cd sxhkd
cp sxhkdrc ~/.config/sxhkd
```
3.2.3.-Ahora con la barra
```
cd ..
cd polybar
cp colors.ini colors_dark.ini color_light.ini config current.ini launch.sh workspace.ini ~/.config/polybar
cd fonts
cp Helvetica_BoldOblique.ttf Helvetica_Bold.ttf helvetica_compressed_5871d14b6903a.otf helvetica_light_587ebe5a59211.ttf 2helvetica_rounded_bold_5871d05ead8de.otf Helvetica.ttf HurmitNerdFontComplete_Mono.otf 'Iosevka Nerd Font Complete.ttf' ~/.config/polybar/fonts
cd ..
cd scripts
cp launcher  powermenu  powermenu_alt ~/.config/polybar/scripts
cd themes
cp colors_dark.rasi colors.rasi powermenu_alt.rasi colors_light.rasi launcher.rasi powermenu.rasi ~/.config/polybar/scripts/themes
cd ~/DotfilesForEverybody/.config
```
3.2.4.-El menú de aplicaciones
```bash
cd rofi
cp config ~/.config/rofi
cd themes
cp onedark.rasi ~/.config/rofi/themes
cd ~/DotfilesForEverybody/.config
```
3.2.5.-El compositor de ventanas picom
```bash
cd picom
cp picom.conf ~/.config/picom
cd ..
```
3.2.6.-El gestor de notificaciones
```bash
cd dunst
cp dunstrc ~/.config/dunst
cd ..
```
3.2.7.-Los fondos de pantalla
```bash
cd ~/DotfilesForEverybody/.wallpaper
cp Architect.png BigSur.jpg Ghibli.jpg RocknSky.jpg Stoic.jpg YWing.png ~/.wallpaper
```
# 4.-Resultado final y algunos EasterEggs
Si copiaste todo bien te debia haber salido algo parecido a esto
<p align="center">
  <img src="https://i.imgur.com/YDQO2bQ.png">
  <img src="https://i.imgur.com/AImpdAj.png">
  <img src="https://i.imgur.com/mnkMygA.png"
</p>

4.1.-EasterEggs
En la carpeta poyo te he dejado algunos scripts que los puedes correr de la siguiente forma:

```bash
cd poyo
por ejemplo para correr el script de unix:
./unix
```
# 5.- Agradecimientos y Dedicatoria
Esta guía esta dedicada a todos aquellos que quienes quieren empezar en los gestores de ventanas pero no saben por donde empezar. Agradezco el apoyo de toda la la comunidad de [Xunix](https://www.facebook.com/groups/xunix.welcome.to.the.heaven) son unos capos.

# 6.-Créditos

Para los fondos de pantalla y la paleta de colores(en la terminal y etc): [Miguel Avila](https://github.com/MiguelRAvila)
Para la barra y efectos de compton: [sudo rice](https://github.com/VaughnValle)


# Te gusto la guía
Hace mucho frío que tal si me invitas un cafesito :3

[![ko-fi](https://www.ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/panaderoxis)

Aquí te dejo mi canal de Youtube para que te guíes más :3

[![](https://raw.githubusercontent.com/VaughnValle/demo/master/yt-badge.png)](https://www.youtube.com/sudo_rice)

Me puedes dar un solsito para mi frugos :3

[![](https://c5.patreon.com/external/logo/become_a_patron_button.png)](https://www.patreon.com/natry_nenvf)
