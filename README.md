# OBS Recording Manager

Plugin natif pour [OBS Studio](https://obsproject.com) qui ajoute une fenetre de gestion apres chaque enregistrement, ainsi qu'un envoi automatique vers Google Drive.

---

## Fonctionnalites

- **Dialogue apres chaque enregistrement** : Choisissez de garder, supprimer ou decider plus tard
- **Trois modes de suppression** :
  - Corbeille Windows (recuperable)
  - Dossier temporaire avec suppression automatique apres le delai configure
  - Suppression definitive immediate
- **Annulation rapide** : Apres une suppression en mode dossier temporaire, un toast apparait pendant 10 secondes pour annuler
- **Envoi vers Google Drive** : Connectez votre compte Google et selectionnez un dossier de destination
- **Interface entierement en francais**, integree dans le style d'OBS

---

## Installation

1. Telechargez le fichier `obs-recording-manager.dll` depuis les [Releases](../../releases/latest)
2. Copiez-le dans le dossier `obs-plugins\64bit\` de votre installation OBS  
   *(par defaut : `C:\Program Files\obs-studio\obs-plugins\64bit\`)*
3. Redemarrez OBS
4. Le plugin se charge automatiquement, accedez aux parametres via **Outils > Recording Manager...**

---

## Configuration Google Drive (optionnel)

1. Dans OBS, ouvrez **Outils > Recording Manager...**
2. Allez dans l'onglet **Google Drive**
3. Cliquez sur **Se connecter a Google Drive**
4. Votre navigateur s'ouvre, connectez-vous a votre compte Google et accordez l'acces
5. Cliquez sur **Choisir...** pour selectionner le dossier de destination
6. Choisissez si l'envoi se fait automatiquement quand vous cliquez sur "Garder"

> Le plugin n'accede qu'aux fichiers qu'il a lui-meme crees (`drive.file`).  
> Aucun mot de passe n'est stocke, seul un token de session est conserve localement.

---

## Compatibilite

| OBS Studio | Windows | Qt    |
|------------|---------|-------|
| 32.x       | 10/11   | 6.8.3 |

---

## Licence

MIT - libre d'utilisation, modification et redistribution.

---

## Confidentialite

Consultez notre [Politique de confidentialite](PRIVACY.md).
