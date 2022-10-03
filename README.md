# [Tokyo Night](https://marketplace.visualstudio.com/items?itemName=enkia.tokyo-night)
[![Preview in vscode.dev](https://img.shields.io/badge/preview%20in-vscode.dev-blue)](https://vscode.dev/theme/enkia.tokyo-night/Tokyo%20Night%20Storm)
[![Version](https://vsmarketplacebadge.apphb.com/version/enkia.tokyo-night.svg)](https://marketplace.visualstudio.com/items?itemName=enkia.tokyo-night)
[![Rating](https://vsmarketplacebadge.apphb.com/rating-star/enkia.tokyo-night.svg)](https://marketplace.visualstudio.com/items?itemName=enkia.tokyo-night)
[![Issues](https://img.shields.io/github/issues/enkia/tokyo-night-vscode-theme)](https://github.com/enkia/tokyo-night-vscode-theme/issues)
<br><br>A clean Visual Studio Code theme that celebrates the lights of Downtown [Tokyo at night.](https://www.google.com/search?q=tokyo+night&newwindow=1&sxsrf=ACYBGNRiOGCstG_Xohb8CgG5UGwBRpMIQg:1571032079139&source=lnms&tbm=isch&sa=X&ved=0ahUKEwiayIfIhpvlAhUGmuAKHbfRDaIQ_AUIEigB&biw=1280&bih=666&dpr=2)
<br><br>**Note:** Many UI elements are intentionally low contrast so as not to distract. I can provide [customization settings](https://code.visualstudio.com/api/references/theme-color) similar to what is shown further down this page to anyone who needs specific text brightened.
<br><br>**Semantic Highlighting:** If you prefer all variables inside functions to be the same color, disable semantic highlighting in settings. Otherwise, parameters used will be dimmer in color. [Submit an issue](https://github.com/enkia/tokyo-night-vscode-theme/issues/new) if you notice anything 'off' with semantic highlighting as I've just recently provided support for it.

## Screenshots
Tokyo Night
![Screenshot - Tokyo Night](https://raw.githubusercontent.com/enkia/tokyo-night-vscode-theme/master/static/ss_tokyo_night.png)

Tokyo Night Storm
![Screenshot - Tokyo Night Storm](https://raw.githubusercontent.com/enkia/tokyo-night-vscode-theme/master/static/ss_tokyo_night_storm.png)

Tokyo Night Light
![Screenshot - Tokyo Night Light](https://raw.githubusercontent.com/enkia/tokyo-night-vscode-theme/master/static/ss_tokyo_day.png)

## Disabling Italics
Paste this into your [settings.json](https://code.visualstudio.com/docs/getstarted/settings#_settings-file-locations) to disable italics.

```javascript
"editor.tokenColorCustomizations": {
    "[Tokyo Night]": { // or "[Tokyo Night Storm]"
        "textMateRules": [{
            "scope": [
                "comment",
                "meta.var.expr storage.type",
                "keyword.control.flow",
                "keyword.control.return",
                "meta.directive.vue punctuation.separator.key-value.html",
                "meta.directive.vue entity.other.attribute-name.html",
                "tag.decorator.js entity.name.tag.js",
                "tag.decorator.js punctuation.definition.tag.js",
                "storage.modifier"
            ],
            "settings": {
                "fontStyle": ""
            }
        }]
    }
}
```
## Customization Settings Examples
#### Higher Contrast Settings
The below can by no means officially represent high contrast but they may serve as a starting point. This assumes that the darker Tokyo Night version is being used. 
```javascript
"workbench.colorCustomizations": {
    "[Tokyo Night]": {
        "foreground": "#959cbd",
        "panelTitle.activeBorder": "#3d59a1",
        "panelTitle.activeForeground": "#bdc7f0",
        "panelTitle.inactiveForeground": "#959cbd",
        "tab.activeForeground": "#bdc7f0",
        "tab.inactiveForeground": "#959cbd",
        "breadcrumb.foreground": "#959cbd",
        "breadcrumb.focusForeground": "#bdc7f0",
        "breadcrumb.activeSelectionForeground": "#bdc7f0",
        "statusBar.foreground": "#bdc7f0",
        "list.focusForeground": "#bdc7f0",
        "list.hoverForeground": "#bdc7f0",
        "list.activeSelectionForeground": "#bdc7f0",
        "list.inactiveSelectionForeground": "#bdc7f0",
        "list.inactiveSelectionBackground": "#202330",
        "sideBar.foreground": "#959cbd",
        "dropdown.foreground": "#959cbd",
        "menu.foreground":"#bdc7f0",
        "menubar.selectionForeground":"#bdc7f0",
        "input.foreground": "#959cbd",
        "input.placeholderForeground": "#959cbd",
        "activityBar.foreground": "#bdc7f0",
        "activityBar.inactiveForeground": "#787c99",
        "gitDecoration.ignoredResourceForeground": "#696d87",
    },
}
```
#### Brightening Codelens text
I prefer my Codelens text fade into the background unless hovered over, but if you'd like a higher contrast, add this to your settings.json:
```javascript
"workbench.colorCustomizations": {
    "[Tokyo Night]": { // or "[Tokyo Night Storm]"
        "editorCodeLens.foreground": "#7982a9", // Preferred hex color
    }
}
```

#### Window Active and Inactive borders (vscode 1.40.0)
macOS dark-mode doesn't play well with these two theme mods so I've chosen to darken them as much as I can to fix the gray border issue on my side. Set them however you like using:
```javascript
"workbench.colorCustomizations": {
    "[Tokyo Night]": { // or "[Tokyo Night Storm]"
        "window.activeBorder": "#ff0000",
        "window.inactiveBorder":"#0000ff"
    }
}
```

## Color Palette
#### Collapse Dark
| Color&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | Use |
| ---------- | ------------------------------------------------------------ |
| ![#f7768e](https://place-hold.it/15/f7768e/f7768e?text=+) `#f7768e` | This keyword, HTML elements, Regex group symbol, CSS units, Terminal Red |
| ![#ff9e64](https://place-hold.it/15/ff9e64/ff9e64?text=+) `#ff9e64` | Number and Boolean constants, Language support constants |
| ![#e0af68](https://place-hold.it/15/e0af68/e0af68?text=+) `#e0af68` | Function parameters, Regex character sets, Terminal Yellow |
| ![#9ece6a](https://place-hold.it/15/9ece6a/9ece6a?text=+) `#9ece6a` | Strings, CSS class names |
| ![#73daca](https://place-hold.it/15/73daca/73daca?text=+) `#73daca` | Object literal keys, Markdown links, Terminal Green |
| ![#b4f9f8](https://place-hold.it/15/b4f9f8/b4f9f8?text=+) `#b4f9f8` | Regex literal strings |
| ![#2ac3de](https://place-hold.it/15/2ac3de/2ac3de?text=+) `#2ac3de` | Language support functions, CSS HTML elements |
| ![#7dcfff](https://place-hold.it/15/7dcfff/7dcfff?text=+) `#7dcfff` | Object properties, Regex quantifiers and flags, Markdown headings, Terminal Cyan, Markdown code, Import/export keywords |
| ![#7aa2f7](https://place-hold.it/15/7aa2f7/7aa2f7?text=+) `#7aa2f7` | Function names, CSS property names, Terminal Blue |
| ![#bb9af7](https://place-hold.it/15/bb9af7/bb9af7?text=+) `#bb9af7` | Control Keywords, Storage Types, Regex symbols and operators, HTML Attributes, Terminal Magenta |
| ![#c0caf5](https://place-hold.it/15/c0caf5/c0caf5?text=+) `#c0caf5` | Variables, Class names, Terminal White |
| ![#a9b1d6](https://place-hold.it/15/a9b1d6/a9b1d6?text=+) `#a9b1d6` | Editor Foreground |
| ![#9aa5ce](https://place-hold.it/15/9aa5ce/9aa5ce?text=+) `#9aa5ce` | Markdown Text, HTML Text |
| ![#cfc9c2](https://place-hold.it/15/cfc9c2/cfc9c2?text=+) `#cfc9c2` | Parameters inside functions (semantic highlighting only) |
| ![#565f89](https://place-hold.it/15/565f89/565f89?text=+) `#565f89` | Comments |
| ![#414868](https://place-hold.it/15/414868/414868?text=+) `#414868` | Terminal Black |
| ![#24283b](https://place-hold.it/15/24283b/24283b?text=+) `#24283b` | Editor Background (Storm) |
| ![#1a1b26](https://place-hold.it/15/1a1b26/1a1b26?text=+) `#1a1b26` | Editor Background (Night) |

#### Collapse Purple
| Color&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | Use |
| ---------- | ------------------------------------------------------------ |
| ![#f7768e](https://place-hold.it/15/f7768e/f7768e?text=+) `#f7768e` | This keyword, HTML elements, Regex group symbol, CSS units, Terminal Red |
| ![#ff9e64](https://place-hold.it/15/ff9e64/ff9e64?text=+) `#ff9e64` | Number and Boolean constants, Language support constants |
| ![#e0af68](https://place-hold.it/15/e0af68/e0af68?text=+) `#e0af68` | Function parameters, Regex character sets, Terminal Yellow |
| ![#9ece6a](https://place-hold.it/15/9ece6a/9ece6a?text=+) `#9ece6a` | Strings, CSS class names |
| ![#73daca](https://place-hold.it/15/73daca/73daca?text=+) `#73daca` | Object literal keys, Markdown links, Terminal Green |
| ![#b4f9f8](https://place-hold.it/15/b4f9f8/b4f9f8?text=+) `#b4f9f8` | Regex literal strings |
| ![#2ac3de](https://place-hold.it/15/2ac3de/2ac3de?text=+) `#2ac3de` | Language support functions, CSS HTML elements |
| ![#7dcfff](https://place-hold.it/15/7dcfff/7dcfff?text=+) `#7dcfff` | Object properties, Regex quantifiers and flags, Markdown headings, Terminal Cyan, Markdown code, Import/export keywords |
| ![#7aa2f7](https://place-hold.it/15/7aa2f7/7aa2f7?text=+) `#7aa2f7` | Function names, CSS property names, Terminal Blue |
| ![#bb9af7](https://place-hold.it/15/bb9af7/bb9af7?text=+) `#bb9af7` | Control Keywords, Storage Types, Regex symbols and operators, HTML Attributes, Terminal Magenta |
| ![#c0caf5](https://place-hold.it/15/c0caf5/c0caf5?text=+) `#c0caf5` | Variables, Class names, Terminal White |
| ![#a9b1d6](https://place-hold.it/15/a9b1d6/a9b1d6?text=+) `#a9b1d6` | Editor Foreground |
| ![#9aa5ce](https://place-hold.it/15/9aa5ce/9aa5ce?text=+) `#9aa5ce` | Markdown Text, HTML Text |
| ![#cfc9c2](https://place-hold.it/15/cfc9c2/cfc9c2?text=+) `#cfc9c2` | Parameters inside functions (semantic highlighting only) |
| ![#565f89](https://place-hold.it/15/565f89/565f89?text=+) `#565f89` | Comments |
| ![#414868](https://place-hold.it/15/414868/414868?text=+) `#414868` | Terminal Black |
| ![#24283b](https://place-hold.it/15/24283b/24283b?text=+) `#24283b` | Editor Background (Storm) |
| ![#1a1b26](https://place-hold.it/15/1a1b26/1a1b26?text=+) `#1a1b26` | Editor Background (Night) |