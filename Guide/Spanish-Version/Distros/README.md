## 2.-Primeros Pasos (Para ditribuciones basadas en Debian: Linux Mint, Ubuntu, Kubuntu, Kali Linux, Lubuntu, ufff y demás)
2.1.- Primeramente actualizaremos el sitema y los repositorios:
```bash
sudo apt-get update && sudo apt-get upgrade
```
2.2.-Luego instalaremos las dependencias que necesitamos para bspwm y sxhkd:
```bash
  sudo apt install build-essential git xcb libxcb-util0-dev libxcb-ewmh-dev libxcb-randr0-dev libxcb-icccm4-dev libxcb-keysyms1-dev libxcb-xinerama0-dev libasound2-dev libxcb-xtest0-dev libxcb-shape0-dev
```
2.3.-Ahora recien instalamos bspwm:
```bash
sudo apt-get install bspwm
```
2.4.-Y luego sxhkd para los atajos de tecla:
```bash
sudo apt-get install sxhkd
```
2.5.-Instalamos las dependencias de polybar(la barrita :3)
```bash
  sudo apt install cmake cmake-data pkg-config python3-sphinx libcairo2-dev libxcb1-dev libxcb-util0-dev libxcb-randr0-dev libxcb-composite0-dev python3-xcbgen xcb-proto libxcb-image0-dev libxcb-ewmh-dev libxcb-icccm4-dev libxcb-xkb-dev libxcb-xrm-dev libxcb-cursor-dev libasound2-dev libpulse-dev libjsoncpp-dev libmpdclient-dev libcurl4-openssl-dev libnl-genl-3-dev
```
2.6.-Instalamos la barra
```bash
   git clone --recursive https://github.com/polybar/polybar
   cd polybar
   mkdir build
   cd build
   cmake ..
   make -j$(nproc)
   sudo make install
```
2.7.-Instalamos las dependencias del menú de aplicaciones
```bash
  sudo apt install bison flex libstartup-notification0-dev check autotools-dev libpango1.0-dev librsvg2-bin librsvg2-dev libcairo2-dev libglib2.0-dev libxkbcommon-dev libxkbcommon-x11-dev libjpeg-dev
  ```
2.8.-Y luego instalamos check (necesario para el menú de aplicaciones)
```bash
  wget https://github.com/davatorium/rofi/releases/download/1.5.4/rofi-1.5.4.tar.gz
  wget https://github.com/libcheck/check/releases/download/0.15.1/check-0.15.1.tar.gz
  cd check-0.15.1
  ./configure
  make
  make check
  sudo make install
  cd ..
```
2.9.-Compilamos rofi
```bash
  cd rofi
  mkdir build && cd build
  ../configure
  make
```
2.10.-Ahora lo instalamos
```bash
  sudo apt-get install rofi
```
2.11.-Instalamos la terminal
```bash
sudo apt-get install kitty
```
2.12.-Instalamos feh para el fondo de pantalla
```bash
sudo apt-get install feh
```
2.13.-Instalamos las dependencias el compositor de ventanas
```bash
  sudo apt install meson libxext-dev libxcb1-dev libxcb-damage0-dev libxcb-xfixes0-dev libxcb-shape0-dev libxcb-render-util0-dev libxcb-render0-dev libxcb-randr0-dev libxcb-composite0-dev libxcb-image0-dev libxcb-present-dev libxcb-xinerama0-dev libpixman-1-dev libdbus-1-dev libconfig-dev libgl1-mesa-dev  libpcre2-dev  libevdev-dev uthash-dev libev-dev libx11-xcb-dev
```
2.14.-Clonamos el repositorio, complilamos e instalamos
```bash
  git clone https://github.com/ibhagwan/picom.git
  cd picom
  git submodule update --init --recursive
  meson --buildtype=release . build
  ninja -C build
  sudo ninja -C build install
  cd ..
```
2.15.-Instalamos el gestionador de notificaciones
```bash
sudo apt-get install dunst
```
