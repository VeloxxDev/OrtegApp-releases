# OrtegApp : téléchargements

Outil de traitement des raws : upscale waifu2x, fusion et découpe des planches.
Disponible sur **Windows** et **Mac**.

Tout se télécharge depuis la dernière version :
**https://github.com/VeloxxDev/OrtegApp-releases/releases/latest**

## Windows

### Installer ou mettre à jour

1. Télécharge `OrtegApp.exe`.
2. Si une ancienne version existe, remplace-la par le nouvel exe. Tes réglages sont conservés.
3. Au premier lancement, Windows peut afficher « Windows a protégé votre ordinateur ».
   Fais un clic droit sur `OrtegApp.exe` > Propriétés > coche « Débloquer » > OK, puis relance.
   Tu peux aussi cliquer sur « Informations complémentaires », puis « Exécuter quand même ».

L'app prévient elle-même quand une nouvelle version sort : un bouton « MISE À JOUR » apparaît en haut.
Il installe la nouvelle version tout seul et relance l'app, avec tes réglages.

### Prérequis

- Windows 10 ou 11 (64 bits).
- Microsoft Edge WebView2, déjà présent sur la plupart des PC. S'il manque, l'app donne le lien pour l'installer.
- Une carte graphique compatible Vulkan. Sans elle, choisis « Processeur » dans Paramètres > GPU (très lent).
- Si le traitement échoue avec « mémoire du GPU insuffisante », règle « Tile size » à 128 dans Paramètres > Performance.

## Mac

### Quel fichier télécharger

Deux versions, selon ton Mac. Pour savoir laquelle : menu Pomme (en haut à gauche) > « À propos de ce Mac ».

- « Puce Apple M1 / M2 / M3… » → télécharge **`OrtegApp-macos-arm64.zip`**.
- « Processeur Intel… » → télécharge **`OrtegApp-macos-x86_64.zip`**.

### Installer

1. Double-clique le `.zip` téléchargé : il se décompresse en `OrtegApp.app`.
2. Glisse `OrtegApp.app` dans ton dossier **Applications**.
3. L'app n'est pas signée par Apple : au premier lancement, macOS la bloque (« impossible d'ouvrir… développeur non identifié »). Pour l'autoriser, une seule fois :
   - Ouvre **Réglages Système** > **Confidentialité et sécurité**.
   - Descends tout en bas : un message cite `OrtegApp`. Clique **« Ouvrir quand même »**, puis confirme.
   - Si le message n'apparaît pas : dans le dossier Applications, fais un **clic droit sur `OrtegApp.app` > Ouvrir**, puis « Ouvrir » dans la fenêtre.

   Autre méthode (Terminal), si le blocage persiste :
   ```
   xattr -dr com.apple.quarantine /Applications/OrtegApp.app
   ```

### Mettre à jour

Sur Mac, la mise à jour n'est **pas** automatique. Quand l'app affiche « MISE À JOUR », le bouton ouvre cette page :
retélécharge le `.zip` de ta version (arm64 ou x86_64) et remplace `OrtegApp.app` dans Applications.

### Prérequis

- Un Mac récent, à puce Apple (M1 et au-delà) ou Intel.
- Le traitement choisit automatiquement le GPU. En cas de souci, choisis « Processeur » dans Paramètres > GPU (très lent).

## Le bouton « ? »

Le bouton « ? » en haut de l'app ouvre cette page d'aide.

## En cas de problème

Envoie le fichier journal :

- **Windows** : `%APPDATA%\OrtegApp\logs\ortegapp.log` — colle ce chemin dans la barre d'adresse de l'Explorateur.
- **Mac** : `~/Library/Application Support/OrtegApp/logs/ortegapp.log` — dans le Finder, menu « Aller » > « Aller au dossier… » (ou ⇧⌘G), colle le chemin.
