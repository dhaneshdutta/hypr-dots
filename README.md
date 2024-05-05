### 💥 Copying / Installation / Update instructions 💥
> [!Note] 
> The auto copy script will create backups of intended folders to be copied. However, still a good idea to manually backup just incase script failed to backup!
- ~/.config (btop cava hypr kitty rofi swappy swaync waybar wlogout) - These are folders to be copied.
- ~/Pictures/wallpapers - Will be backed up
- clone this repo by using git. Change directory, make executable and run the script
```bash
git clone --depth=1 https://github.com/dhaneshdutta/hypr-dots.git
cd hypr-dots
```
- to copy/install from upstream (possible bugs)
```bash
chmod +x copy.sh
./copy.sh
```
- to copy/install from releases (more "stable")
```bash
chmod +x release.sh
./release.sh
```

- UPGRADE.sh (Experimental)
> [!IMPORTANT]
> You should atleast v2.2.3 in your hyprland dots (ls ~/.config/hypr) to check version
> You need rsync for it to work

> [!CAUTION]
> you should have already up and running Hyprland before using this function
```bash
chmod +x upgrade.sh
./upgrade.sh
```

#### 🛎️ a small note on wallpapers
- by default, only few wallpapers will be copied (1 each dark and light plus 2 more). You will be offered to download more wallpapers. You can preview/check the additional wallpapers on [`THIS`](https://github.com/JaKooLit/Wallpaper-Bank/tree/main/wallpapers) Link


#### ⚠️⚠️⚠️ A MUST! after copying  / Installing these dots

+ By default I have not set a wallpaper. Press SUPER W and set a wallpaper. This is also to initiate pywal for waybar, kitty (tty) and rofi themes. If you use the copy.sh script, you wont need to do this.

+ Nvidia Owners. Make sure to edit your `~/.config/hypr/UserConfigs/ENVariables.conf` (recommended). Below env's will be activated if automatic copy is used
> WLR_NO_CURSORS,1 , LIBVA_DRIVER_NAME,nvidia ,  __GLX_VENDOR_LIBRARY_NAME,nvidia 
- NVIDIA users / owners, after installation, check [`THIS`](https://github.com/JaKooLit/Hyprland-Dots/wiki/Notes_to_remember#--for-nvidia-gpu-users)

+ If you have already set your own keybinds, monitors, etc.... Just copy over from backup created before log-out or reboot. (recommended)        
