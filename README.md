# Instructions

1. Installer l'extension `Custom CSS and JS loader`
2. Copier le contenu de `settings.json` dans le dossier `User` de VSCode (Attention : ça va remplacer les paramètres actuels)
3. Ajouter le tableau `vs_code_css.imports` dans le ficheier `settings.json` pour ajouter des fichiers CSS personnalisés

```json
"vscode_custom_css.imports": [
    // Absolute file paths for your css/js files
    // For Mac or Linux
    // "file:///Users/your-user-name/custom-vscode.css"
    // "file:///Users/your-user-name/custom-vscode-script.js"

    // For Windows
    // "file:///C:/path-of-custom-css/custom-vscode.css"
    // "file:///C:/path-of-custom-css/custom-vscode-script.js"
],
```

4. Vous devrez peut-être prendre possession des fichiers CSS/JS que vous avez créés ou exécuter VS Code avec des privilèges administratifs sur certains systèmes d'exploitation :

```md
Mac and Linux users
The extension would NOT work if Visual Studio Code cannot modify itself. The cases include:

Code files being read-only, like on a read-only file system or,
Code is not started with the permissions to modify itself.
You need to claim ownership on Visual Studio Code's installation directory, by running this command:

Note: Replace /usr/share/code where your VS Code is installed.
sudo chown -R your-user-name /usr/share/code
```

5. Activez "Custom CSS and JS Loader" depuis le dialogue de commande de VS Code.
6. Personnalisez le CSS ou le JS de ce dépôt pour le rendre comme vous le souhaitez, ou mieux encore, explorez les zones de VS Code que vous souhaitez personnaliser.
7. Après avoir effectué des changements, rechargez l'extension (Reload Custom CSS and JS) depuis le dialogue de commande de VS Code.
