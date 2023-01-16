# Plugin Pipup

Plugin permettant de créer une notification sur Android TV via PiPup.

# Prérequis

Le plugin est basé sur une application AndroidTV : PiPup. (https://github.com/rogro82/PiPup)

En résumé :
- Installer sur la TV l'application PiPup, 
- Sur son PC ou son MAC, il faut récupérer l'outil adb (https://developer.android.com/studio/releases/platform-tools)
- Puis via une ligne de commande, se connecter à sa TV
  adb connect <IPTV>
  Vérification :
  adb devices
- Donner les droits d'afficher une popup sur la TV pour cette application :
  adb shell appops set nl.rogro82.pipup SYSTEM_ALERT_WINDOW allow


# Configuration des équipements

La configuration des équipements PiPup est accessible à partir du menu Plugins puis Communication.

Une fois dessus vous retrouvez alors la liste de vos équipements.

## Général

Vous retrouvez ici toute la configuration de votre équipement :

    Nom de l’équipement : nom de votre équipement AndroidTV.
    Objet parent : indique l’objet parent auquel appartient l’équipement.
    Catégorie : les catégories de l’équipement (il peut appartenir à plusieurs catégories).
    Activer : permet de rendre votre équipement actif.
    Visible : le rend visible sur le dashboard.

## Informations

Cet onglet permet de définir l'équipement :

   IP TV : IP de l'équipement où afficher les notifications
   Duration : Durée en seconde pendant laquelle la notification s'affiche. 30 secondes par défaut.
   Position : Emplacement où s'afficheront les notifications. En bas à droite par défaut.
   Taille du titre : 20 par défaut
   Taille du message : 14 par défaut
   Taille de l'image : 240 par défaut

## Commandes

Commandes créées pour voir des informations :

    notify : affiche une notification de type Notify
    alert : affiche une notification de type Alert

Les commandes sont personnalisables :

   Title color : couleur du titre
   Message color : couleur du texte du message
   Background color : couleur de fond
   URL : URL de l'image. Si vide, il n'y a pas d'image affichée.
      Exemple :
      https://www.pinclipart.com/picdir/big/85-851186_push-notifications-push-notification-icon-png-clipart.png
      https://www.pinclipart.com/picdir/big/94-941341_open-animated-gif-alert-icon-clipart.png
      https://jeannedarcroye.files.wordpress.com/2019/01/attention-2.gif
      Un GIF animé peut être choisi.
