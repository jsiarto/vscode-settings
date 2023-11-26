# VS Code
Settings, themes, and customizations for Visual Studio Code

## Theme
I use a _lightly_ customized version of the popular [Dracula](https://draculatheme.com) theme. My modifictions are listed in the `settings.json` configuration below. Make sure to [install the theme in VS Code](https://draculatheme.com/visual-studio-code) before applying `workbench.colorCustomizations` and `editor.tokenColorCustomizations` to your `settings.json`.

### Modifications
- Creates a dark, solid background line highlight in the editor.
- Changes the green in the attribute name property to #40F99B.

## settings.json
```json
{
    "editor.fontSize": 16,
    "editor.cursorStyle": "block",
    "editor.wordWrap": "on",
    "breadcrumbs.enabled": false,
    "editor.hover.enabled": false,
    "git.confirmSync": false,
    "editor.codeActionsOnSave": {

    },
    "editor.accessibilitySupport": "off",
    "workbench.colorTheme": "Dracula",
    "editor.minimap.enabled": false,
    "editor.fontWeight": "normal",
    "editor.tabSize": 2,
    "workbench.tips.enabled": false,
    "workbench.colorCustomizations": {
        "editor.lineHighlightBackground": "#191A21",
        "editor.lineHighlightBorder": "#191A21"
    },
    "editor.tokenColorCustomizations": {
        "[Dracula]": {
            "textMateRules": [
                {
                    "scope": "entity.other.attribute-name",
                    "settings": {
                        "foreground": "#40F99B",
                    }             
                }
            ]
        }
    },
}
```
