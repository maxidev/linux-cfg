# Linux Configuration

A comprehensive collection of packages, tools, and configuration files for setting up a productive Linux environment.

## Overview

This repository contains configuration files and installation instructions for setting up a Linux environment based on Linux Mint (Sarah Cinnamon edition). It includes essential packages, shell configuration, themes, and productivity tools.

## Table of Contents

- [Base Installation](#base-installation)
- [Shell Setup](#shell-setup)
- [Terminal Customization](#terminal-customization)
- [Development Tools](#development-tools)
- [Media Tools](#media-tools)
- [Customization](#customization)

## Base Installation

Install essential packages for development and system management:

```bash
sudo apt-get install build-essential htop ccze iptraf nmap guake gir1.2-gtop-2.0 tmux \
                     clipit unrar zip unzip p7zip-full p7zip-rar rar tree netcat git httpie
```

## Shell Setup

### Fish Shell

Fish is a smart and user-friendly shell with syntax highlighting, autosuggestions, and more.

```bash
sudo apt-get install fish
```

To set Fish as your default shell:

```bash
chsh -s $(which fish)
```

### Fisher Package Manager

Fisher is a plugin manager for Fish:

```bash
curl -sL https://raw.githubusercontent.com/jorgebucaran/fisher/main/functions/fisher.fish | source && fisher install jorgebucaran/fisher
```

### Tide Prompt for Fish

Install the Tide prompt theme for Fish:

```bash
fisher install IlanCosman/tide@v6
```

## Terminal Customization

### Fonts

Several fonts are recommended for optimal terminal experience:

#### MesloLGS NF (for Tide and Powerline)

Download and install the following font files:
- [MesloLGS NF Regular](https://github.com/IlanCosman/tide/blob/assets/fonts/mesloLGS_NF_regular.ttf?raw=true)
- [MesloLGS NF Bold](https://github.com/IlanCosman/tide/blob/assets/fonts/mesloLGS_NF_bold.ttf?raw=true)
- [MesloLGS NF Italic](https://github.com/IlanCosman/tide/blob/assets/fonts/mesloLGS_NF_italic.ttf?raw=true)
- [MesloLGS NF Bold Italic](https://github.com/IlanCosman/tide/blob/assets/fonts/mesloLGS_NF_bold_italic.ttf?raw=true)

To install these fonts:
1. Download the font files
2. Double-click each file to open it in the font viewer
3. Click "Install" for each font
4. Set the font in your terminal preferences

#### Additional Fonts

Install the TypeCatcher font manager to access Google Fonts:

```bash
sudo apt-get install typecatcher
```

[Inconsolata](http://levien.com/type/myfonts/inconsolata.html) is also recommended for programming.

### Powerline Shell

For a customized terminal prompt with Git integration and system information:

Follow the installation guide: [powerline-installation](https://github.com/maxidev/powerline-installation)

### Tmux Configuration

Create or edit `~/.tmux.conf`:

```bash
set-option -g prefix M-a
set -g status off

# make tmux display things in 256 colors
set -g default-terminal "screen-256color"

# set scrollback history to 10000 (10k)
set -g history-limit 10000
```

## Development Tools

All essential development packages are included in the base installation. Additional language-specific tools can be installed as needed.

## Media Tools

### MOC Player Theme

Set up a dark theme for MOC music player:

```bash
touch ~/.moc/config && echo "Theme = nightly_theme" > ~/.moc/config
```

## Customization

Add any other customization options and themes here.

## Gnome Extensions

Enhance your Gnome desktop environment with these useful extensions:

```bash
# List of recommended Gnome extensions
extensions/auto-power-profile@dmy3k.github.io/
extensions/bluetooth-quick-connect@bjarosze.gmail.com/
extensions/blur-my-shell@aunetx/
extensions/clipboard-indicator@tudmotu.com/
extensions/ddterm@amezin.github.com/
extensions/grand-theft-focus@zalckos.github.com/
extensions/impatience@gfxmonk.net/
extensions/just-perfection-desktop@just-perfection/
extensions/openbar@neuromorph/
extensions/power-profile@fthx/
extensions/Vitals@CoreCoding.com/
```

You can install these extensions from the [Gnome Extensions website](https://extensions.gnome.org/) or by using the Gnome Extensions app:

```bash
sudo apt install gnome-shell-extensions gnome-shell-extension-manager
```

### Extension Descriptions

- **Auto Power Profile**: Automatically switches power profiles based on battery status
- **Bluetooth Quick Connect**: Adds quick connect/disconnect options to Bluetooth devices
- **Blur My Shell**: Adds a blur effect to different parts of the Gnome shell
- **Clipboard Indicator**: Clipboard manager extension for Gnome
- **DDTerm**: Drop-down terminal for Gnome
- **Grand Theft Focus**: Prevents applications from stealing focus
- **Impatience**: Speeds up Gnome Shell animations
- **Just Perfection**: Customizes Gnome Shell elements
- **OpenBar**: Enhances the top bar functionality
- **Power Profile**: Easily switch between power profiles
- **Vitals**: System monitoring extension

## Usage

1. Clone this repository:
   ```bash
   git clone https://github.com/maxidev/linux-cfg.git
   ```

2. Navigate to the repository:
   ```bash
   cd linux-cfg
   ```

3. Follow the installation instructions in each section according to your needs.

## License

This project is open-source and free to use.