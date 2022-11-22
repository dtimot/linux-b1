# Première machine

Changer le hash du mot de passe du root et des users dans le dossier /etc/shadow
La commande utilisée est donc (sudo si on est pas en root) nano /etc/shadow

```
Lors du login meme en rescue mode on ne peut pas se login
```

# Deuxième machine
Remove le grub en suprimant le fichier grub.cfg 
La commande utilisée est donc (sudo si on est pas en root) rm /boot/grub2/grub.cfg
```
il n'y a plus de grub donc on ne peut pas se connecter
```

# Troisième machine
Supprimer le bin 
La commande utilisée est donc (sudo si on est pas en root) rm /bin 

# Quatrième machine

changer la langue locale avec ces 3 commandes:
>sudo yum search langpacks
>sudo yum install langpacks-ru.noarch
>sudo localectl set-locale LANG=ru_RU.utf8

changer le langage du clavier avec celles là
>localectl list-keymaps
>localectl set-keymap cz-rus
```
les caractères sont floutés et les caractères ne sont pas les mêmes donc impossible de se login 
```
