# bspwm-installation-guide

On installe d'abord toutes les nécessités
```shell 
sudo pacman -Syy bspwm sxhkd kitty nitrogen picom lightdm lightdm-gtk-greeter firefox pcmanfm dmenu xorg
```

On va créer les fichiers config qui contient les règles de nos outils. On va du coup pouvoir les modifier et customiser à notre guise notre affichage avec ces fichiers

On crée les répertoires qui contiennent les fichiers config
```shell
mkdir .config
mkdir .config/bspwm
mkdir .config/sxhkd
mkdir .config/polybar
```

On copie ensuite les modèles de fichier config donnés dans ce repertoire qu'on vient de créer
```shell
cp /usr/share/doc/bspwm/examples/bspwmrc .config/bspwm
cp /usr/share/doc/bspwm/examples/sxhkdrc .config/sxhkd
```

On va éditer les règles de bspwmrc pour ajouter l'éxecution de sxhkd au début

```
vim .config/bspwm/bspwmrc
```
Vous devriez avoir quelque chose comme ça:

![alt text](bspwmrc_config_1.png)