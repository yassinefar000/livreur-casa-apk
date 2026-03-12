# Livreur Casa APK

Application Android minimale qui ouvre la Web App Livreur Casa dans une WebView.

## Ce que fait cette app

- ouvre directement la Web App livreur
- masque le navigateur pour donner un rendu plus proche d'une application
- gère le retour Android
- ouvre les liens `tel:` dans l'application téléphone
- ouvre les liens WhatsApp dans WhatsApp

## Build sans Android Studio

Le build est prévu via GitHub Actions.

Après chaque push sur `main`, GitHub génère automatiquement un APK debug.

## Où récupérer l'APK

1. Ouvrir l'onglet `Actions` du repo GitHub
2. Ouvrir le dernier workflow `Build APK`
3. Télécharger l'artifact `livreur-casa-debug-apk`

## Mises à jour

La WebView ouvre l'URL Apps Script suivante :

`https://script.google.com/macros/s/AKfycbz7BRfJZ4bFLe9bIRM4KiQ5JuQrL74ySbbW-O__85HaWn94lth4E6aNyzkJF4Nt68g5aQ/exec?v=50`

Donc :

- si vous modifiez la Web App Apps Script, l'APK reflète automatiquement ces changements
- si vous modifiez le code Android lui-même, il faudra reconstruire et renvoyer un nouvel APK
