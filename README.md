# Lab2: Android Rooting
## Objectif
Réaliser un laboratoire de sécurité Android afin de comprendre :
- le rooting,
- Verified Boot / AVB,
- les impacts sécurité.
## Environnement
- Android Studio
- AVD (API 31)
- ADB
## Étape 1 : Rooter l’AVD
![Étape 1 - adb root](screenshots/10.png)
L’émulateur Android (AVD) a été détecté correctement par ADB.  La commande `adb root` permet de redémarrer le service ADB avec des privilèges élevés, ce qui est autorisé uniquement sur les images d’émulateur ou de laboratoire.  La commande `adb shell id` retourne `uid=0 (root)`, confirmant que l’environnement est bien rooté.  Cela permet d’accéder à des zones normalement protégées du système afin d’observer l’impact du root sur les mécanismes de sécurité Android etla commande `fastboot oem device-info` n’est applicable que sur un appareil physique connecté en mode fastboot avec un bootloader déverrouillé.  
## Étape 2 : Fiche périmètre
- Application : App de test (debug)
- Support : Android Virtual Device (AVD)
- Objectif : Comprendre le rooting et ses impacts
- Données : Fictives uniquement
- Réseau : Environnement de test isolé
  
