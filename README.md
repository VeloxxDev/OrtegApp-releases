# OrtegApp : téléchargements

Outil de traitement des raws : upscale waifu2x, fusion et découpe des planches.

## Installer ou mettre à jour

1. Télécharge `OrtegApp.exe` depuis la dernière version :
   **https://github.com/VeloxxDev/OrtegApp-releases/releases/latest**
2. Si une ancienne version existe, remplace-la par le nouvel exe. Tes réglages sont conservés.
3. Au premier lancement, Windows peut afficher « Windows a protégé votre ordinateur ».
   Fais un clic droit sur `OrtegApp.exe` > Propriétés > coche « Débloquer » > OK, puis relance.
   Tu peux aussi cliquer sur « Informations complémentaires », puis « Exécuter quand même ».

L'app prévient elle-même quand une nouvelle version sort : un bouton « MISE À JOUR » apparaît en haut.

## Prérequis

- Windows 10 ou 11 (64 bits).
- Microsoft Edge WebView2, déjà présent sur la plupart des PC. S'il manque, l'app donne le lien pour l'installer.
- Une carte graphique compatible Vulkan. Sans elle, choisis « Processeur » dans Paramètres > GPU (très lent).
- Si le traitement échoue avec « mémoire du GPU insuffisante », règle « Tile size » à 128 dans Paramètres > Performance.

## En cas de problème

Envoie le fichier `%APPDATA%\OrtegApp\logs\ortegapp.log` : colle ce chemin dans la barre d'adresse de l'Explorateur Windows pour l'ouvrir.
