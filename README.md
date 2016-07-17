linux-config
=========

##Packages and configurations.

###Version: Linux Mint Sarah Cinnamon edition

####Base Packages

	sudo apt-get install build-essential htop ccze iptraf nmap guake gir1.2-gtop-2.0 tmux clipit unrar zip unzip p7zip-full p7zip-rar rar tree netcat git httpie

####Media Packages

	sudo apt-get install clementine moc smplayer thunderbird filezilla dropbox kazam

####Nvidia Drivers install

	sudo add-apt-repository ppa:xorg-edgers/ppa
	sudo apt-get update
	sudo apt-get install nvidia-352 nvidia-setting
	
###Configurations


####Fish Shell
	
	sudo apt-get install fish

	Oh-my-fish: 	curl -L https://github.com/oh-my-fish/oh-my-fish/raw/master/bin/install | fish

	theme: omf install bobthefish

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

#### Keepassx PPA

	sudo add-apt-repository ppa:eugenesan/ppa
	sudo apt-get update
	sudo apt-get install keepassx

#####Bitcoin

	sudo apt-add-repository ppa:bitcoin/bitcoin

#####Synapse launcher

	sudo apt-add-repository ppa:synapse-core/testing

#####TLP Power Manager

	sudo apt-get remove laptop-mode-tools
	
	sudo add-apt-repository ppa:linrunner/tlp
	sudo apt-get update 
	sudo apt-get install tlp tlp-rdw
	
	sudo apt-get install smartmontools ethtool
	
	Si tu equipo es un ThinkPad, además deberás instalar los siguientes paquetes adicionales,
	
	sudo apt-get install tp-smapi-dkms acpi-call-tools 
	
	sudo tlp start

#### Cinnamon Applets

	Applets: 'CPU Temperature Indicator' 'Simple Memory Monitor'

	
