# 🌿 HEBDO SANTE USENGHOR - Évaluation de Plateforme

Un formulaire d'évaluation interactif et moderne conçu pour collecter les avis des étudiants de l'Université Senghor sur la plateforme de nutrition **HEBDO SANTE**.

Ce projet inclut :
- Un formulaire HTML/CSS/JS responsive et accessible.
- Une intégration automatique avec Google Sheets (via Apps Script).
- Une gestion du consentement et de la confidentialité.
- Une page de remerciement dédiée.
- Un système de blocage anti-spam (localStorage).

---

## 🚀 Déploiement Rapide

### Prérequis
- Un compte Google (pour Google Sheets & Apps Script).
- Un éditeur de texte (VS Code, Bloc-notes, etc.).
- Un navigateur moderne (Chrome, Firefox, Edge).

### Étape 1 : Configuration de la Base de Données (Google Sheets)

1. Créez une nouvelle **Google Sheet** vierge.
2. Ouvrez **Extensions** > **Apps Script**.
3. Collez le code fourni dans le fichier `script.gs` (ou copiez le code du bloc "Script Google" ci-dessous).
4. Cliquez sur **Déployer** > **Nouveau déploiement**.
   - Type : **Web App**.
   - Exécuter en tant que : **Moi**.
   - Qui peut accéder : **Tout le monde**.
5. Copiez l'**URL du Web App** (elle doit se terminer par `/exec`).

### Étape 2 : Configuration du Formulaire (HTML)

1. Ouvrez le fichier `index.html`.
2. Repérez la ligne :
   ```javascript
   const GOOGLE_SCRIPT_URL = 'https://script.google.com/macros/s/TON_ID_DE_DEPLOIEMENT_ICI/exec';
