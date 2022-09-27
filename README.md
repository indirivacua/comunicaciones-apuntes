# comunicaciones-apuntes

### Configuración VSCode:
* Instalar Extensiones:
  * [Markdown Preview Github Styling](https://marketplace.visualstudio.com/items?itemName=bierner.markdown-preview-github-styles)
  * ~~[Markdown PDF](https://marketplace.visualstudio.com/items?itemName=yzane.markdown-pdf)~~
  * [Markdown+Math](https://marketplace.visualstudio.com/items?itemName=goessner.mdmath)
  * [Markdown All in One](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one)

#### settings.json

    {
        "telemetry.telemetryLevel": "off",
        "editor.tabSize": 2,
        "mdmath.macros": {
          "\\eqref": "\\href{###1}{(\\text{#1})}",
          "\\ref": "\\href{###1}{\\text{#1}}",
          "\\label": "\\htmlId{#1}{}"
        },
        "mdmath.katexoptions": {
            "trust": "(context) => ['\\htmlId', '\\href'].includes(context.command)"
        },
        "mdmath.theme": "publication",
        "markdown.extension.math.enabled": false
    }

### Comandos Útiles:

* <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>V</kbd>: Markdown: Open Preview
* <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>P</kbd>: Command Palette
  * Markdown: Save Markdown+Math to HTML
  * Markdown All in One: Create/Update Table of Contents

### Links Útiles:
* **https://latex.codecogs.com/eqneditor/editor.php**
* https://katex.org/docs/supported.html
* https://katex.org/docs/autorender.html
* https://goessner.github.io/mdmath/publication.html