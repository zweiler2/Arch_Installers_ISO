# How to use the ISO:
Flash the ISO from [releases](https://github.com/zweiler2/Arch_Installers_ISO/releases) using [BalenaEtcher](https://etcher.balena.io), [Rufus](https://rufus.ie) with DD mode, simply throwing the ISO onto a [Ventoy](https://www.ventoy.net) drive or by typing `sudo dd if=Arch_Installers_ISO.iso of=/dev/sd(your flash drive) bs=4M status=progress oflag=sync`  
In case you need to start the script manually just type: Arch_Installers

# How to build the ISO:
```
sudo pacman -Syu --needed archiso
git clone https://github.com/zweiler2/Arch_Installers_ISO.git
sudo mkarchiso -rv ./Arch_Installers_ISO
sudo chown -hR "$USER":"$USER" ./out 
```
Once it finishes, your ISO will be available in the `out` directory.