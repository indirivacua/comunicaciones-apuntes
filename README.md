# comunicaciones-apuntes

Configuración VSCode:
* Instalar extensiones:
* https://marketplace.visualstudio.com/items?itemName=bierner.markdown-preview-github-styles
https://marketplace.visualstudio.com/items?itemName=yzane.markdown-pdf
https://marketplace.visualstudio.com/items?itemName=goessner.mdmath
https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one

Comandos útiles:

* <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>V</kbd>: vista previa del documento
* <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>P</kbd>: Abrir comandos
  * Markdown All-In-One: Create/Update Table of Contents
  * Markdown: Save Markdown+Math to HTML

Links útiles:
https://latex.codecogs.com/eqneditor/editor.php
https://katex.org/docs/autorender.html
https://goessner.github.io/mdmath/publication.html
https://katex.org/docs/supported.html

Settings json

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