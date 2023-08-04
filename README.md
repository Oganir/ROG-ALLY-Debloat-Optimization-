# ROG-ALLY-Debloat-Optimization-

tout dans ce guide est VOTRE PROPRE RISQUE je ne suis responsable de rien.

Avant tout, vous allez avoir besoin de plusieurs choses :
- une clé USB de minimum 16GB
- un hub USB-C avec 3 entrée USB-A
- clavier
- souris


Tout d'abord, il faut mettre a jour et installer TOUS les drivers disponible via MYASUS/ArmoryCrate/WindowsUpdate.
Je conseille d'installer également tous les drivers presents sur la page des drivers pour la ROG ALLY ci-dessous.

https://rog.asus.com/gaming-handhelds/rog-ally/rog-ally-2023/helpdesk_download/


Il est impératif de faire ça car nous allons Backup tous les drivers pour les modifications suivantes.
Une fois que vous êtes pret, créez un dossier "drivers" dans le disque C: a sa base.
le chemin vers ce dossier sera donc "C:\drivers"

Nous allons maintenant utiliser la commande suivante pour backup tous les drivers.
Lancez le terminal windows avec les droits d'administrateurs et coller cette ligne :


dism /online /export-driver /destination:"C:\drivers"

Maintenant nous allons créer une clé USB Bootable
utilisant la verson allegée de windows 11 "GhostSpectre Superlite SE"

Suivez la procédure fournie par le créateur via ce lien :

https://ghostclouds.xyz/wp/w11-22h2-22621/

Telechargez la version 13, installez egalement Rufus & 7-zip sur leur site respectif.

- https://rufus.ie/fr/#
- https://www.7-zip.org

L'iso de GhostSpectre Superlite SE est compressée au forma .U13
Il faut extraire L'iso via 7-zip et mettez la où vous voulez.
Le mot de passe : 22h2u13

Créer ensuite une clé USB bootable de l'iso avec Rufus, laissez les parametres par défaut.

Quand la clé usb bootable est prète, collez le dossier "c:\drivers" a la racine de la clé usb.
Ca nous permettra de pouvoir les réinstaller une fois GhostSpectre Superlite SE installé.

Avant de pouvoir démarrer l'installation il faut désactiver les paramètres suivant dans le Bios de votre ROG ALLY :

- Fastboot
- Secureboot

Pour faire ceci, redémarrez votre Ally et maintenez le bouton volume - lorsque que le logo animé commence au démarrage.

Voici les deux options a désactiver :


![IMG_5015](https://github.com/Oganir/ROG-ALLY-Debloat-Optimization-/assets/141415073/f5b81703-1cdf-4662-881f-8f75f684116b)
![IMG_5016](https://github.com/Oganir/ROG-ALLY-Debloat-Optimization-/assets/141415073/c186c217-dc9d-413a-8650-b19c8d7a47b5)

Enregistrez et quittez.

Redémarrez dans le bios a nouveau, Vous pourrez maintenant choisir la clé usb bootable dans les option de démarrage visible en bas de l'écran.

Vous pouvez suivre les instructions de cette video pour plus de facilités lors de l'installation de l'os :

https://youtu.be/iSoxPFaXBn0?t=510

Selectionnez bien la version Superlite SE ou Superlite SE + WD si vous désirez garder Windows Defender.
Quand l'installation est effectuée, félicitations vous avez fait la base de votre nouvel OS !

Nous devons maintenant importer tous les drivers essentiels pour la ROG-Ally.
Pour cela, copiez et coller le dossier drivers de votre clé usb à la racine de votre disque C: 
Il faut ouvrir Powershell entant qu'administrateur et coller la ligne de commande suivante :

pnputil /add-driver "C:\drivers\*.inf" /subdirs /install /reboot

Laissez powershell faire sa magie et redémarrez votre ROG-ALLY


Superlite SE n'a pas de navigateur installé par défaut ( bye Edge ) il faut donc démarrer Ghost Toolbolx qui est sur votre bureau et installer le navigateur de votre choix.
Par exemple pour Chrome, faites 14 sur votre clavier puis enter (il est impératif d'etre connecté à internet pour cela).
Je recommande également de faire les options 16 et 17.

![image](https://github.com/Oganir/ROG-ALLY-Debloat-Optimization-/assets/141415073/a2b96bd0-adc7-4959-a444-b4c9ef6b16b6)


Il faut également activer le Touch Keyboard.
Pour ceci faites l'option 20 puis 3 et redémarrez.
Vous pourrez ensuite l'activer via les paramètres windows, réglez les comme ci-dessous.

![image](https://github.com/Oganir/ROG-ALLY-Debloat-Optimization-/assets/141415073/ba4a934f-22be-42e4-8da3-eec4836693e6)

Il faut ensuite installer Armoury Crate. Rien de plus simple appuyez sur le bouton de votre Rog Ally pour le lancer, une fenetre s'ouvre, vous pourez le télécharger et l'installer.

Notre Base est désormait prète et fonctionnelle.
Je recommande également d'utiliser l'outil de Chris pour completer notre optimisation.

https://github.com/ChrisTitusTech/winutil

suivez ses indications et une fois l'outil ouvert, cochez ces options dans "Tweaks":

![image](https://github.com/Oganir/ROG-ALLY-Debloat-Optimization-/assets/141415073/cd4f8e3b-3d26-43b0-8bbb-1037360e0358)

cliquez sur Run Tweaks, quand il aura terminé, redémarez votre Rog-ALLY.

Je recommande la création d'un dossier "Games" à la racine de votre disque C: où vous installerez tous vos jeux et game launcher (Steam,GoG,..) avant de faire l'option suivante.
Nous allons compresser notre installation de windows via les options de Ghost toolbox. 

il faut donc démarrer Ghost Toolbox qui est sur votre bureau et choisir l'option 9 puis 1.

![image](https://github.com/Oganir/ROG-ALLY-Debloat-Optimization-/assets/141415073/a2b96bd0-adc7-4959-a444-b4c9ef6b16b6)
![image](https://github.com/Oganir/ROG-ALLY-Debloat-Optimization-/assets/141415073/369768ad-6c6b-4109-9d42-a95aca3a510e)

L'opération peut prendre plus de 10 minutes, ne touchez a rien pendant l'opération et gardez la ROG ally branchée.

Redémarrez encore une fois votre ROG ally une fois l'opération terminée.

Si vous désirez ce style de bureau :

![image](https://github.com/Oganir/ROG-ALLY-Debloat-Optimization-/assets/141415073/6e8876bb-f4b6-4afb-a02a-1c12a582b69d)

Faites clic droit sur votre barre de tâche, propriétés et configurez les options comme ceci ( j'ai régler la résolution sur 720P personellement):

![image](https://github.com/Oganir/ROG-ALLY-Debloat-Optimization-/assets/141415073/901fe9ef-31b0-4577-ae70-361e8afda9f9)
![image](https://github.com/Oganir/ROG-ALLY-Debloat-Optimization-/assets/141415073/96854cc0-b640-48ed-a70d-6afd82c2eec8)
![image](https://github.com/Oganir/ROG-ALLY-Debloat-Optimization-/assets/141415073/aab06634-b0a8-4e12-aee4-d85d6856c613)

N'oubliez pas de désactiver les programmes au démarrage si vous n'en avez pas besoin comme steam, chrome,...
La création de profils personalisés dans Armoury crate est également recommandée. voici les miens à titre d'exemple :

![image](https://github.com/Oganir/ROG-ALLY-Debloat-Optimization-/assets/141415073/491f6742-11d1-4bb9-849f-003b1a323cf7)
![image](https://github.com/Oganir/ROG-ALLY-Debloat-Optimization-/assets/141415073/b629669a-9333-49b8-889c-af4de94c9506)
![image](https://github.com/Oganir/ROG-ALLY-Debloat-Optimization-/assets/141415073/b3ae0018-9848-444b-99f2-da364e1d6cae)

Votre ROG est désomais optimisée et ne sera pas ralentie par Windows.


















