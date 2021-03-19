<h1 align="center">Personalización en Arch</h1>

3.1.-Empecemos con los ficheros base así que tienes que clonar este repositorio (Estos pasos se aplican tanto para los usuarios de distros basadas en Arch y Debian)
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
