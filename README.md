# Native macOS Theme

Native macOS is a color theme for [Visual Studio Code](https://code.visualstudio.com) that aims to match native macOS applications as closely as possible. The extension includes four versions - two light and two dark, with a light and a dark editor version for each.

**Native macOS - Light Theme**
![Light theme, light editor](/images/light-theme-light-editor.png "Light theme, light editor")
<figcaption>The "Light theme, light editor" variant</figcaption>

![Light theme, dark editor](/images/light-theme-dark-editor.png "Light theme, dark editor")
<figcaption>The "Light theme, dark editor" variant</figcaption>

![Dark theme, light editor](/images/dark-theme-light-editor.png "Dark theme, light editor")
<figcaption>The "Dark theme, light editor" variant</figcaption>

![Dark theme, dark editor](/images/dark-theme-dark-editor.png "Dark theme, dark editor")
<figcaption>The "Dark theme, dark editor" variant</figcaption>

## Optional Tweaks

There are a few optional tweaks you can do to really nail down the look of native macOS. The native title bar, for example, really makes a huge difference, and so does the font, SF Mono (you can find that [here](https://developer.apple.com/fonts/), if you don't already have it installed). You can easily perform these tweaks by using the command pallette to open `settings.json` (`Shift` + `Ctrl` + `P` on Windows, `Shift` + `⌘` + `P` on Mac) and searching "Preferences".

```json
"window.titleBarStyle": "native",
"window.nativeTabs": true
"editor.fontSize": 12,
"editor.fontFamily": "SF Mono, Monaco",
"editor.tabSize": 2,
"editor.fontWeight": "normal"
```

You can also hide the Activity bar and replace it with an extension like [Activitus Bar](https://marketplace.visualstudio.com/items?itemName=Gruntfuggly.activitusbar) to further the look, and use an extension like [Vibrancy](https://marketplace.visualstudio.com/items?itemName=eyhn.vscode-vibrancy) to complete it.

```json
"workbench.activityBar.visible": false,
 "vscode_vibrancy.theme": "Dark (Only Subbar)",
"vscode_vibrancy.type": "menu",
"vscode_vibrancy.opacity": 0
```

If you'd like, you can also disable to minimap, though I personally prefer to keep mine on for ease of use.

```json
"editor.minimap.enabled": false
```

To complete the look, you can also replace the default icon of Visual Studio Code with one of the macOS-themed icons included. `icon.png` will work on both macOS and Windows, and `icon.icns` and `icon.ico` will work exclusively on each one respectively.

## To replace the application icon on macOS

The easiest option is to use an application like [LiteIcon](https://freemacsoft.net/liteicon/) to replace the default icon. If you'd rather do it yourself, however, read on.

Navigate to your applications folder and find Visual Studio Code. Right-click on it, then click "Show Package Contents". From here, navigate to **Contents**, then to **Resources**, then delete **Code.icns**. You will replace this icon with the custom icon included.

Navigate to the Visual Studio Code extensions folder (`Users/your-name/.vscode/extensions`)<sup>[1](#hidden-folders)</sup>. Find the Native macOS Theme Folder (`dsoloha.native-macos-0.0.1`), then right-click `icon.icns` and click "Duplicate". Rename the duplicate to "Icon.icns" and drag it into the Visual Studio Code Resources folder from earlier.

Restart Visual Studio Code. Remove it from your dock and re-add it, if necessary.

## To replace the program icon on Windows

Open the directory in which you installed Visual Studio Code (`C:\users\{username}\AppData\Local\Programs\Microsoft VS Code` by default). Right-click the `VSCode.exe` executable, then click **Properties**, then press the **Change Icon** button. From here, navigate to the Visual Studio Code extensions directory (`%USERPROFILE%\.vscode\extensions` by default). Double-click on `icon.ico`.

Restart Visual Studio Code.

<sup id="hidden-folders">1</sup> If the `.vscode` folder isn't showing, press `Shift` + `⌘` + `.` to show your hidden folders.
