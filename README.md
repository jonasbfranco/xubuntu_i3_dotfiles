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
> 15&nbsp;&nbsp;&nbsp;=&nbsp;&nbsp;&nbsp;lxappearance



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


#### ⚙ Como utilizar meus arquivos 
> Baixe os arquivos 
* 1 . [Baixe os arquivos ](https://github.com/jonasbfranco/xubuntu_i3_dotfiles.git) git clone https://github.com/jonasbfranco/xubuntu_i3_dotfiles.git   
* 2 . Extraia os arquivos em seus respectivos locais apos ter instalado os passos a seguir.



#### ⚙ 1 Passo - Instalar Powerline
> https://github.com/powerline/powerline  
> * $sudo apt install powerline  
> * $sudo mkdir /usr/local/bin/powerline  
> * $sudo git clone https://github.com/powerline/powerline.git /usr/local/bin/powerline  
> * $sudo wget https://github.com/powerline/powerline/raw/develop/font/PowerlineSymbols.otf -O /usr/share/fonts/PowerlineSymbols.otf  
> * $sudo wget https://github.com/powerline/powerline/raw/develop/font/10-powerline-symbols.conf -O /etc/fonts/conf.d/10-powerline-symbols.conf  
> * $sudo echo '. /usr/local/bin/powerline/powerline/bindings/bash/powerline.sh' >> ~/.bashrc  


#### ⚙ 2 Passo - Instalar os programas abaixo (opcional)

> * cava
> * sudo apt-get install libfftw3-dev libasound2-dev libncursesw5-dev libpulse-dev libtool -y && wget  http://ppa.launchpad.net/tehtotalpwnage/ppa/ubuntu/pool/main/c/cava/cava_0.6.0-0ubuntu3_amd64.deb && sudo dpkg -i cava* 
> * [Download Cava](https://github.com/jonasbfranco/xubuntu_i3_dotfiles/raw/master/programas/cava_0.6.0-0ubuntu3_amd64.deb)
> * Para instalar
> * sudo dpkg -i cava_0.6.0-0ubuntu3_amd64.deb

> * tty-clock -C7
> * sudo apt install tty-clock
 
> * neofetch [Link](https://github.com/dylanaraps/neofetch)
> * sudo apt install neofetch

> * Spotify (instalation = $sudo snap install spotify)


![Print of Desktop](https://raw.github.com/jonasbfranco/xubuntu_i3_dotfiles/master/desktop.png)

![Print of Desktop - Spotify](https://raw.github.com/jonasbfranco/xubuntu_i3_dotfiles/master/spotify.png)



#### ⚙ 3 Passo - Instalar i3 gaps

sudo apt install git libxcb1-dev libxcb-keysyms1-dev libpango1.0-dev libxcb-util0-dev libxcb-icccm4-dev libyajl-dev libstartup-notification0-dev libxcb-randr0-dev libev-dev libxcb-cursor-dev libxcb-xinerama0-dev libxcb-xkb-dev libxkbcommon-dev libxkbcommon-x11-dev autoconf libxcb-xrm0 libxcb-xrm-dev automake libxcb-shape0-dev -y && git clone https://www.github.com/Airblader/i3 i3-gaps && cd i3-gaps && autoreconf --force --install && rm -rf build/ && mkdir -p build && cd build/ && ../configure --prefix=/usr --sysconfdir=/etc --disable-sanitizers && make && sudo make install
>

#### ⚙ 4 Passo - Instalar polybar

sudo apt-get install cmake cmake-data libcairo2-dev libxcb1-dev libxcb-ewmh-dev libxcb-icccm4-dev libxcb-image0-dev libxcb-randr0-dev libxcb-util0-dev libxcb-xkb-dev pkg-config python-xcbgen xcb-proto libxcb-xrm-dev libasound2-dev libmpdclient-dev libiw-dev libcurl4-openssl-dev libpulse-dev libxcb-composite0-dev xcb libxcb-ewmh2 -y && git clone https://github.com/jaagr/polybar.git && cd polybar && sudo ./build.sh


#### ⚙ 5 Passo - Configurar arquivos necessarios

sudo chown -R $USER:$USER ~/.config/polybar && wget https://gitlab.com/terminalroot/popy/raw/master/launch.sh -O ~/.config/polybar/launch.sh && chmod +x ~/.config/polybar/launch.sh && echo -e 'for_window [class="^.*"] border pixel 0\ngaps inner 10\ngaps outer 2\nexec_always --no-startup-id $HOME/.config/polybar/launch.sh' >> ~/.config/i3/config


#### ⚙ 6 Passo - Opcinal - EU NAO INSTALEI - Instalar Albert

sudo sh -c "echo 'deb http://download.opensuse.org/repositories/home:/manuelschneid3r/xUbuntu_18.04/ /' > /etc/apt/sources.list.d/home:manuelschneid3r.list" && wget -nv https://download.opensuse.org/repositories/home:manuelschneid3r/xUbuntu_18.04/Release.key -O Release.key && sudo apt-key add - < Release.key && sudo apt-get update && sudo apt-get install albert -y

* Rode no terminal albert Configure o Hotkey, aplicativos, temas, …;
* Abra o arquivo de configuração do i3 e comente a linha que contém dmenu: vi ~/.config/i3/config;
* Adicione a linha albert & no final do arquivo: vi ~/.config/polybar/launch.sh;
* Remova o alsa do painel do Polybar: vi ~/.config/polybar/config;
* Reinicie o i3: Super + shift + r.


#### ⚙ 7 Passo - Instalar Cava

sudo apt-get install libfftw3-dev libasound2-dev libncursesw5-dev libpulse-dev libtool -y && wget http://ppa.launchpad.net/tehtotalpwnage/ppa/ubuntu/pool/main/c/cava/cava_0.6.0-0ubuntu3_amd64.deb && sudo dpkg -i cava*



#### ⚙ 8 Passo - Instalando feh

sudo apt install feh

Instalação
Para instalar o feh, basta usar seu gerenciador de pacotes, exemplo pro APT: sudo apt install feh

Utilizando
Quando você roda o feh feh caminho/para/imagem.jpg pela primeira vez, ele cria automágicamente um arquivo Shell Script no seu diretório pessoal com o nome .fehbg , ou seja, pra vc reutilizar basta rodar esse script.

Isso é interessante quando você deseja manter o papel de parede que você definiu sempre presente, sem precisar ficar rodando toda hora o mesmo comando, essa é a técnica usada para arquivos do [i3wm](echo 'exec $HOME/.fehbg' >> ~/.config/i3/config) , para o bspwm e até mesmo pro seu ~/.xinitc, ~/.xprofile, ~/.bashrc, ~/.profile e outros se você utilizá-los.


Exemplo do conteúdo do meu ~/.fehbg , ou seja, possui o caminho do meu último comando executado:

cat ~/.fehbg

#!/bin/sh
feh --bg-scale '/home/marcos/Imagens/wallpapers/terminalroot-wallpaper-089.jpg'

Lista de opções via linha de comando
A opção que eu mais uso que é justamente que tem no exemplo do meu ~/.fehbg citado acima é:

feh --bg-scale caminho/para/imagem.png - Essa opçao coloca o arquivo em segundo plano sem repeti-lo, cortando coisas ou usando bordas. Mas a proporção também não é preservada.
Outras opções:

feh -g 640x480 -d -S nome-da-minha-imagem Imagens/ - Procura imagens no diretório indicado (Nesse caso em ~/Imagens/) e automáticamente abre ela na proporção 640x480 como o nome nome-da-minha-imagem
--no-fehbg - Desabilita por padrão a criação ou alteração do arquivo ~/.fehbg
--bg-fill - preserva a proporção, ampliando a imagem até que ela caiba. Uma parte horizontal ou vertical da imagem será cortada. É semelhante à opção --bg-scale , a única diferença é que com scale mantém a proporção da imagem.
--bg-tile - Mosaico , repete a imagem, caso ela seja muito pequena para a tela.

 
--bg-center - Centraliza a imagem em segundo plano. Se for muito pequena, será cercado por uma borda, conforme especificado por --image-bg;
--randomize - Gera papéis de paredes randômicos para seu Desktop, geralmente usa em conjunto com alguma parâmetro –bg-[tipo] , exemoplo: feh --randomize --bg-scale ~/Imagens/wallpapers/*.
--recursive - Uma imagem para cada área de trabalho do seu Desktop, randômicamente, ou seja, usa em conjunto com a opção --randomize, exemplo: feh --recursive --randomize --bg-scale ~/Imagens/wallpapers/*

Além diversas de outras possibilidades bem bacanas que podem ser consultadas dando uma olhada mais detalhada ainda no manual: man feh , se você rodar feh --help ele vai mandar você ver o manual! =)






#### ⚙ Creditos Terminal Root
[Link dos Comandos](https://terminalroot.com.br/2019/01/ubuntu-i3gaps-albert-cava-polybar.html "Site Terminal Root")



