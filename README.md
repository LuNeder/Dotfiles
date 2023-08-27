# Dotfiles
On this repository you'll find the dotfiles for my desktop

![Captura de tela_2023-08-25_21-32-56](https://github.com/LuNeder/Dotfiles/assets/19750714/c95488b9-aced-486a-9ee3-a42a3b5770dd)
![Captura de tela_2023-08-25_21-36-31](https://github.com/LuNeder/Dotfiles/assets/19750714/1ac4a3ca-8df3-4448-93f3-6ee1a96ced68)
![Captura de tela_2023-08-25_21-37-07](https://github.com/LuNeder/Dotfiles/assets/19750714/76f33937-5a73-4248-bed6-e4c0b433b085)
![Captura de tela_2023-08-25_21-37-40](https://github.com/LuNeder/Dotfiles/assets/19750714/eb5486dd-773d-4062-a4a6-2148efa9d913)
![Captura de tela_2023-08-25_22-01-36](https://github.com/LuNeder/Dotfiles/assets/19750714/f2d8b72a-b0f9-42fa-8280-bbc538ff9359)



## What's here?
- Compiz
- Emerald
- XFCE
- Polybar
- Rofi
- Maybe more

## Dependencies
Make sure you have installed
- Compiz, Emerald and its plugins:
  ```bash
  sudo zypper in compiz compiz-branding-openSUSE compiz-emerald compiz-emerald-theme-manager compiz-emerald-themes compiz-manager compiz-plugins compiz-plugins-experimental compiz-plugins-extra compiz-plugins-main compizconfig-settings-manager python311-compizconfig
  ```
- XFCE
- Polybar: `sudo zypper in polybar`
- Rofi: `sudo zypper in rofi`
- [adi1090x's themes for Rofi](https://github.com/adi1090x/rofi)
- ULauncher
- Plank
- [feather font](https://github.com/adi1090x/polybar-themes/blob/master/fonts/feather.ttf)
- Maybe something else I forgot

## Instaling
- Make sure you've installed all dependencies and that they're all working properly
- Make compiz your default compositor
  ```bash
  xfconf-query -c xfce4-session -p /sessions/Failsafe/Client1_Command -t string -sa xfsettingsd

  xfconf-query -c xfce4-session -p /sessions/Failsafe/Client0_Command -t string -s compiz -t string -s ccp

  ```
- Move Polybar's `config.ini` file to `~/.config/polybar/` and `.restpolymain` to your home
- Move (and replace) Rofi's `launcher.sh` and `style-1.rasi` to `~/.config/rofi/launchers/type-3/`
- Open CompizConf and import Compiz's file. You'll have to change skydome settings to point to the `80894-360render.jpeg` image you downloaded
- Add `polybar main` to you XFCE's startup programs on settings
- Import the xfce-panel file into your xfce-panel backup page
- The Plank configuration is basically default
- Configure keyboard shortcuts as you please
- I think that's it!


