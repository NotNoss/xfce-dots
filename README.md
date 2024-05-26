# XFCE Dot Files

# THIS README IS NOT COMPLETE AND WILL NOT LEAD TO A COMPLETE INSTALL. USE AT YOUR OWN RISK!

## Welcome to my XFCE4 Dot Files
Below you will find a list of applications that will need to be installed prior to setting up the dot files.
None of these are required unless you want an exact copy of my setup.

```
Brave Web Browser
Kitty
Picom
Spicetify (and Spotify)
Thunar
Discord
Vencord
ZSH
```

Below are also helpful links for setting up the theme.
If I forgot any, I will upload the link here.

[New Tab Redirect](https://chromewebstore.google.com/detail/new-tab-redirect/icpgjfneehieebagbmdbhnlpiopdcmna)
[Tokyonight XFCE Theme](https://github.com/Fausto-Korpsvart/Tokyo-Night-GTK-Theme)
[Papirus Icon Theme](https://github.com/PapirusDevelopmentTeam/papirus-icon-theme)
[Vencord Theme](https://betterdiscord.app/theme/Tokyo%20Night)
[Tokyonight Browser Theme](https://chromewebstore.google.com/detail/tokyonight/enpfonmmpgoinjpglildebkaphbhndek)

## Installation
```bash
sudo pacman -S kitty picom thunar spotify-launcher discord zsh
yay -S brave-bin spicetify-cli
sh -c "$(curl -sS https://raw.githubusercontent.com/Vendicated/VencordInstaller/main/install.sh)"
```

```bash
git clone https://github.com/NotNoss/xfce-dots.git ~/.config/dotfiles
ln -s ~/.config/dotfiles/kitty ~/.config/kitty
ln -s ~/.config/dotfiles/picom ~/.config/picom
ln -s ~/.config/spicetify/TokyoNight-spicetify ~/.config/spicetify/Themes/TokyoNight-spicetify
rm -f ~/.config/xfce4/xfconf/xfce-perchannel-xml/xfce4-panel.xml
ln -s ~/.config/dotfiles/xfce/panel/xfce4-panel.xml ~/.config/xfce4/xfconf/xfce-perchannel-xml/xfce4-panel.xml
rm -f ~/.config/dotfiles/.zshrc ~/.zshrc
```