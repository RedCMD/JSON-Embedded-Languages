# JSON Embedded Languages
Syntax Highlighting for embedded languages within `JSON` and `JSONC` files.  
It does so by overriding the default `JSON` and `JSONC` languages and assigning scopeNames to objects with the form `.meta.embedded.object-key-name.`.  
Then using multiple injection grammars that target and inject specific languages into it.  


## Features
* ShellScript within `"scripts"` for `package.json` (`JSON`)  
  Requires the builtin `ShellScript` extension or [better-shell-syntax](https://marketplace.visualstudio.com/items?itemName=jeff-hykin.better-shellscript-syntax)  
![Example `package.json`](images/Example-Scripts.png)

* Regular Expressions within `"wordPattern"`, `"folding"`, `"onEnterRules"` and `"indentationRules"` for `language-configuration.json` (`JSONC`)  
  Requires [JSON TextMate](https://marketplace.visualstudio.com/items?itemName=RedCMD.tmlanguage-syntax-highlighter) extension  
![Example `language-configuration.json`](images/Example-language-configuration.png)

* Snippets, Regex and Markdown within `"defaultSnippets"`, `"pattern"` and `"markdownDescription"` for `.schema.json` (`JSON`)  
  Requires the builtin `JSON Snippets` extension or [Snippets Snippets](https://marketplace.visualstudio.com/items?itemName=RedCMD.snippets-snippets), [JSON TextMate](https://marketplace.visualstudio.com/items?itemName=RedCMD.tmlanguage-syntax-highlighter) and the builtin `Markdown` extension  
![Example `schema.json`](images/Example-schema.png)


## Known Issues

This extension targets every `JSON` and `JSONC` file, not just `package.json`.  
There will be false positives and false negatives.  
Please report any you come across.  


## For more information

* The GitHub [Issue](https://github.com/microsoft/vscode/issues/224581) that spawned the idea
* [Repository](https://github.com/RedCMD/JSON-Embedded-Languages)
* [Marketplace](https://marketplace.visualstudio.com/items?itemName=RedCMD.json-embedded-languages)


## TODO:
* `package.json`/`"when"`
* `package.json`/`"problemMatchers"`/`"regexp"`
* `globs`/`"filenamePatterns"`
* switch JSON escaped oniguruma regex for JSON escaped JavaScript regex
