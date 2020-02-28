<p align='center'><b>Repositório de:</b> Jonas B. Franco | @jonasbfranco<br>
<b>Email:</b> <a href='mailto:jonasbfranco@gmail.com'>jonasbfranco@gmail.com</a><br>
<b>Site:</b> <a href='https://jonasbfranco.github.io/'>Navegar pelo site (em construcao)</a></p>

<p align='center'><br> Dotfiles Xubuntu i3 </p>


![Print of Desktop](https://raw.github.com/jonasbfranco/xubuntu_i3_dotfiles/master/desktop.png)

### Programas utilizados
> 01&nbsp;&nbsp;&nbsp;=&nbsp;&nbsp;&nbsp;cava  
> 02&nbsp;&nbsp;&nbsp;=&nbsp;&nbsp;&nbsp;Xfce4-Terminal  
> 03&nbsp;&nbsp;&nbsp;=&nbsp;&nbsp;&nbsp;tty-clock  
> 04&nbsp;&nbsp;&nbsp;=&nbsp;&nbsp;&nbsp;pulseaudio  
> 05&nbsp;&nbsp;&nbsp;=&nbsp;&nbsp;&nbsp;pulseaudio-alsa  
> 06&nbsp;&nbsp;&nbsp;=&nbsp;&nbsp;&nbsp;polybar  
> 07&nbsp;&nbsp;&nbsp;=&nbsp;&nbsp;&nbsp;openweather  
> 08&nbsp;&nbsp;&nbsp;=&nbsp;&nbsp;&nbsp;spotify  
> 09&nbsp;&nbsp;&nbsp;=&nbsp;&nbsp;&nbsp;popcorn  
> 10&nbsp;&nbsp;&nbsp;=&nbsp;&nbsp;&nbsp;telegram  
> 11&nbsp;&nbsp;&nbsp;=&nbsp;&nbsp;&nbsp;mailspring  
> 12&nbsp;&nbsp;&nbsp;=&nbsp;&nbsp;&nbsp;neofetch   
> 13&nbsp;&nbsp;&nbsp;=&nbsp;&nbsp;&nbsp;sublime-text  
> 14&nbsp;&nbsp;&nbsp;=&nbsp;&nbsp;&nbsp;visual studio  
> 14&nbsp;&nbsp;&nbsp;=&nbsp;&nbsp;&nbsp;lxappearance



### Configuração dos Workspaces
> 01&nbsp;&nbsp;&nbsp;=&nbsp;&nbsp;&nbsp;Home  
> 02&nbsp;&nbsp;&nbsp;=&nbsp;&nbsp;&nbsp;Terminal  
> 03&nbsp;&nbsp;&nbsp;=&nbsp;&nbsp;&nbsp;Firefox    
> 04&nbsp;&nbsp;&nbsp;=&nbsp;&nbsp;&nbsp;Arquivos    
> 05&nbsp;&nbsp;&nbsp;=&nbsp;&nbsp;&nbsp;Spotify    
> 06&nbsp;&nbsp;&nbsp;=&nbsp;&nbsp;&nbsp;Steam    
> 07&nbsp;&nbsp;&nbsp;=&nbsp;&nbsp;&nbsp;Telegram    
> 08&nbsp;&nbsp;&nbsp;=&nbsp;&nbsp;&nbsp;Desenvolvimento       
> 09&nbsp;&nbsp;&nbsp;=&nbsp;&nbsp;&nbsp;Desktop     
> 10&nbsp;&nbsp;&nbsp;=&nbsp;&nbsp;&nbsp;Mail     


### Customizacoes
> 01&nbsp;&nbsp;&nbsp;=&nbsp;&nbsp;&nbsp;Powerline  
> 02&nbsp;&nbsp;&nbsp;=&nbsp;&nbsp;&nbsp;Neofetch  
> 03&nbsp;&nbsp;&nbsp;=&nbsp;&nbsp;&nbsp;Polybar  


#### ⚙ 1° Como utilizar meus arquivos 
> Baixe os arquivos 
* 1 . [Baixe os arquivos ](https://github.com/jonasbfranco/xubuntu_i3_dotfiles.git) git clone https://github.com/jonasbfranco/xubuntu_i3_dotfiles.git   
* 2 . Extraia os arquivos em seus respectivos locais


#### ⚙ Instalar Powerline
> https://github.com/powerline/powerline  

> * $sudo pacman -S powerline  
> * $sudo apt install powerline  
> * $sudo mkdir /usr/local/bin/powerline  
> * $sudo git clone https://github.com/powerline/powerline.git /usr/local/bin/powerline  
> * $sudo wget https://github.com/powerline/powerline/raw/develop/font/PowerlineSymbols.otf -O /usr/share/fonts/PowerlineSymbols.otf  
> * $sudo wget https://github.com/powerline/powerline/raw/develop/font/10-powerline-symbols.conf -O /etc/fonts/conf.d/10-powerline-symbols.conf  
> * $sudo echo '. /usr/local/bin/powerline/powerline/bindings/bash/powerline.sh' >> ~/.bashrc  


#### ⚙ Prints

> * cava
> * tty-clock -C7
> * neofetch [Link](https://github.com/dylanaraps/neofetch)


> * Spotify (instalation = $sudo snap install spotify)

![Print of Desktop - Spotify](https://raw.github.com/jonasbfranco/xubuntu_i3_dotfiles/master/spotify.png)



#### ⚙ Opções extras de instalação

> * Instalar i3 gaps

sudo apt install git libxcb1-dev libxcb-keysyms1-dev libpango1.0-dev libxcb-util0-dev libxcb-icccm4-dev libyajl-dev libstartup-notification0-dev libxcb-randr0-dev libev-dev libxcb-cursor-dev libxcb-xinerama0-dev libxcb-xkb-dev libxkbcommon-dev libxkbcommon-x11-dev autoconf libxcb-xrm0 libxcb-xrm-dev automake libxcb-shape0-dev -y && git clone https://www.github.com/Airblader/i3 i3-gaps && cd i3-gaps && autoreconf --force --install && rm -rf build/ && mkdir -p build && cd build/ && ../configure --prefix=/usr --sysconfdir=/etc --disable-sanitizers && make && sudo make install


> * Instalar polybar

sudo apt-get install cmake cmake-data libcairo2-dev libxcb1-dev libxcb-ewmh-dev libxcb-icccm4-dev libxcb-image0-dev libxcb-randr0-dev libxcb-util0-dev libxcb-xkb-dev pkg-config python-xcbgen xcb-proto libxcb-xrm-dev libasound2-dev libmpdclient-dev libiw-dev libcurl4-openssl-dev libpulse-dev libxcb-composite0-dev xcb libxcb-ewmh2 -y && git clone https://github.com/jaagr/polybar.git && cd polybar && sudo ./build.sh


> * Configurar arquivos necessarios

sudo chown -R $USER:$USER ~/.config/polybar && wget https://gitlab.com/terminalroot/popy/raw/master/launch.sh -O ~/.config/polybar/launch.sh && chmod +x ~/.config/polybar/launch.sh && echo -e 'for_window [class="^.*"] border pixel 0\ngaps inner 10\ngaps outer 2\nexec_always --no-startup-id $HOME/.config/polybar/launch.sh' >> ~/.config/i3/config


> * Instalar Albert

sudo sh -c "echo 'deb http://download.opensuse.org/repositories/home:/manuelschneid3r/xUbuntu_18.04/ /' > /etc/apt/sources.list.d/home:manuelschneid3r.list" && wget -nv https://download.opensuse.org/repositories/home:manuelschneid3r/xUbuntu_18.04/Release.key -O Release.key && sudo apt-key add - < Release.key && sudo apt-get update && sudo apt-get install albert -y

* Rode no terminal albert Configure o Hotkey, aplicativos, temas, …;
* Abra o arquivo de configuração do i3 e comente a linha que contém dmenu: vi ~/.config/i3/config;
* Adicione a linha albert & no final do arquivo: vi ~/.config/polybar/launch.sh;
* Remova o alsa do painel do Polybar: vi ~/.config/polybar/config;
* Reinicie o i3: Super + shift + r.


> * Instalar Cava

sudo apt-get install libfftw3-dev libasound2-dev libncursesw5-dev libpulse-dev libtool -y && wget http://ppa.launchpad.net/tehtotalpwnage/ppa/ubuntu/pool/main/c/cava/cava_0.6.0-0ubuntu3_amd64.deb && sudo dpkg -i cava*



#### ⚙ Creditos Terminal Root
[Link dos Comandos](https://terminalroot.com.br/2019/01/ubuntu-i3gaps-albert-cava-polybar.html)





