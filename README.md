linux-config
=========

##Packages and configurations.

###Version: Linux Mint 17 Qiana x64 Cinnamon edition

####Base Packages


	sudo apt-get install build-essential htop ccze iptraf nmap guake tmux  unrar zip unzip p7zip-full p7zip-rar rar tree netcat

####Media Packages

	sudo apt-get install clementine moc smplayer qbittorrent google-chrome-stable thunderbird filezilla irssi shutter

####Programming Packages

	sudo apt-get install git nodejs npm dropbox sublime-text atom vim

####Optional Packages

	sudo apt-get install virtualbox shotwell network-manager-openvpn-gnome skype apache2-utils


###Configurations

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


####PPAs

	sudo apt-add-repository ppa:bitcoin/bitcoin

#### Cinnamon Applets


	Applets: 'CPU Temperature Indicator' 'Github Explorer' 'Multi-core System Monitor'
	'Simple Memory Monitor'

####Cinnamon Desklets

	Desklets: 'Weather Desklet (Rosario AR - code: 3838583)' - 'Sticky Notes'
