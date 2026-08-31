# OBS Recording Manager

Plugin natif pour [OBS Studio](https://obsproject.com) qui ajoute une fenêtre de gestion après chaque enregistrement, ainsi qu'un envoi automatique vers Google Drive.

---

## Fonctionnalités

- **Dialogue après chaque enregistrement** — Choisissez de garder, supprimer ou décider plus tard
- **Trois modes de suppression** :
  - Corbeille Windows (récupérable)
  - Dossier temporaire avec suppression automatique après le délai configuré
  - Suppression définitive immédiate
- **Annulation rapide** — Après une suppression en mode dossier temporaire, un toast apparaît pendant 10 secondes pour annuler
- **Envoi vers Google Drive** — Connectez votre compte Google et sélectionnez un dossier de destination
- **Interface entièrement en français**, intégrée dans le style d'OBS

---

## Installation

1. Téléchargez le fichier `obs-recording-manager.dll` depuis les [Releases](../../releases/latest)
2. Copiez-le dans le dossier `obs-plugins\64bit\` de votre installation OBS  
   *(par défaut : `C:\Program Files\obs-studio\obs-plugins\64bit\`)*
3. Redémarrez OBS
4. Le plugin se charge automatiquement — accédez aux paramètres via **Outils → Recording Manager…**

---

## Configuration Google Drive (optionnel)

1. Dans OBS, ouvrez **Outils → Recording Manager…**
2. Allez dans l'onglet **☁ Google Drive**
3. Cliquez sur **Se connecter à Google Drive**
4. Votre navigateur s'ouvre — connectez-vous à votre compte Google et accordez l'accès
5. Cliquez sur **Choisir…** pour sélectionner le dossier de destination
6. Choisissez si l'envoi se fait automatiquement quand vous cliquez sur « Garder »

> Le plugin n'accède qu'aux fichiers qu'il a lui-même créés (`drive.file`).  
> Aucun mot de passe n'est stocké — seul un token de session est conservé localement.

---

## Compilation depuis les sources

**Prérequis :** Visual Studio 2022 (workload Desktop C++), CMake ≥ 3.16, OBS Studio installé

```powershell
git clone https://github.com/chardclouzi/obs-recording-manager
cd obs-recording-manager
.\build.ps1 -Install
```

Le script télécharge automatiquement les en-têtes OBS et Qt6, génère les bibliothèques d'import et installe le plugin.

---

## Compatibilité

| OBS Studio | Windows | Qt   |
|-----------|---------|------|
| 32.x      | 10/11   | 6.8.3|

---

## Licence

MIT — libre d'utilisation, modification et redistribution.

---

## Confidentialité

Consultez notre [Politique de confidentialité](PRIVACY.md).
