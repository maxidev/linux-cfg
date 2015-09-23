linux-config
=========

##Packages and configurations.

###Version: Linux Mint 17.2 Rafaela Cinnamon edition

####Base Packages

	sudo apt-get install build-essential htop ccze iptraf nmap guake gir1.2-gtop-2.0 tmux clipit unrar zip unzip p7zip-full p7zip-rar rar tree netcat git

####Media Packages

	sudo apt-get install clementine moc smplayer thunderbird filezilla dropbox

####Optional Packages

	sudo apt-get install virtualbox shotwell network-manager-openvpn-gnome vim

####Nvidia Drivers install

	sudo add-apt-repository ppa:xorg-edgers/ppa
	sudo apt-get update
	sudo apt-get install nvidia-352 nvidia-setting
	
####Plank Dock

	sudo add-apt-repository ppa:ricotz/docky # <- is not a typo
	sudo apt-get update
	sudo apt-get install plank

###Configurations

####Grub Customizer

	sudo add-apt-repository ppa:danielrichter2007/grub-customizer
	sudo apt-get update
	sudo apt-get install grub-customizer

####Fonts

	sudo apt-get install typecatcher

Inconsolata (for programming): http://levien.com/type/myfonts/inconsolata.html


####Virtualbox Shared Folders

	sudo adduser xxxxxxx vboxsf to solve 'permission denied' on folder opening

####MOC player dark theme

	touch ~/.moc/config && echo "Theme = nightly_theme" > ~/.moc/config

####GTK Theme

Delorean-Dark-Green (3.6-g) https://launchpad.net/~killhellokitty/+archive/themes.ppa


####Powerline Shell

Follow this guide: https://github.com/maxidev/powerline-installation

####Tmux Conf (edit or create ~/.tmux.conf)

	set-option -g prefix M-a                                                                   
	set -g status off                                                                          
	# use UTF8                                                                                 
	set -g utf8                                                                                
	set-window-option -g utf8 on                                                               
	                                                                                           
	# make tmux display things in 256 colors                                                   
	set -g default-terminal "screen-256color"                                                  
	                                                                                           
	# set scrollback history to 10000 (10k)                                                    
	set -g history-limit 10000

####PPAs

#####Bitcoin
	sudo apt-add-repository ppa:bitcoin/bitcoin

#####Synapse launcher
	sudo apt-add-repository ppa:synapse-core/testing

#####TLP Power Manager

	sudo add-apt-repository ppa:linrunner/tlp
	sudo apt-get update
	sudo apt-get install tlp tlp-rdw
	sudo tlp start

#### Cinnamon Applets


	Applets: 'CPU Temperature Indicator' 'Github Explorer' 'Multi-core System Monitor'
	'Simple Memory Monitor'

####Cinnamon Desklets

	Desklets: 'Weather Desklet (Rosario AR - code: 3838583)' - 'Sticky Notes'
	
####FIX Google Chrome bad icon

	sudo nano /usr/share/applications/google-chrome.desktop
	Add: StartupWMClass=Google-chrome-stable to each entry
	

