# VS Code - settings.json

## How to apply custom styles to your VS Code

1. Install "Custom CSS and JS Loader" VS Code Extension.

2. Copy the contents of settings.json to your VS Code's settings.json (warning: it will overwrite your settings).

3. Add `vscode_custom_css.imports` array to your settings.json file:

```
"vscode_custom_css.imports": [
    // Absolute file paths for your css/js files
    // For Mac or Linux
    // "file:///Users/your-user-name/style.css",
    // "file:///Users/your-user-name/script.js"

    // For Windows
    // "file:///C:/path-of-custom-css/style.css",
    // "file:///C:/path-of-custom-js/script.js"
],
```

4. You might need to take ownership of the CSS/JS files you made or run VS Code with admin privileges on certain operating system:

```
Mac and Linux users
The extension would NOT work if Visual Studio Code cannot modify itself. The cases include:

Code files being read-only, like on a read-only file system or,
Code is not started with the permissions to modify itself.
You need to claim ownership on Visual Studio Code's installation directory, by running this command:

Note: Replace /usr/share/code where your VS Code is installed.
sudo chown -R your-user-name /usr/share/code
```

5. Enable "Custom CSS and JS Loader" from VS Code's command dialog.

6. Customize the css or js from this repo to make it look the way you want to, or even better, explore areas of VS Code that you want to customize.

7. After making some changes, reload the extension (Reload Custom CSS and JS) from VS Code's command dialog.
