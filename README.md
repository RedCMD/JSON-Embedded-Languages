# JSON Embedded Languages
Syntax Highlighting for embedded languages within `JSON` and `JSONC` files.  
It does so by overriding the default `JSON` and `JSONC` languages and assigning a scopeName to each object with the form `.meta.embedded.objectkey.`.  
Then using multiple injection grammars that target those scopeNames and inject specific languages into it.  


## Features
* ShellScript within `"scripts"` for `package.json` (`JSON`)  
![Example `package.json/scripts`](images/Example-scripts.png)

* [when-clause-contexts](https://code.visualstudio.com/api/references/when-clause-contexts) within `"when"` for `package.json` (`JSON`)  
![Example `package.json/when`](images/Example-when.png)

* JSON escaped JavaScript Regular Expressions within `"wordPattern"`, `"folding"`, `"onEnterRules"` and `"indentationRules"` for `language-configuration.json` (`JSONC`)  
![Example `language-configuration.json`](images/Example-language-configuration.png)

* Snippets, Regex and Markdown within `"defaultSnippets"`, `"pattern"` and `"markdownDescription"` for `.schema.json` (`JSON`)  
  Recommend the [Snippets Snippets](https://marketplace.visualstudio.com/items?itemName=RedCMD.snippets-snippets) extension  
![Example `schema.json`](images/Example-schema.png)


## Known Issues

This extension targets every `JSON` and `JSONC` file, not just `package.json`.  
There will be false positives and false negatives.  
Please report any you come across.  

VSCode TextMate injections are rather slow.  
It may take longer for documents to fully syntax highlight.  
The `regexp` `"injectionSelector"` is almost 10,000 characters long.  


## For more information

* The GitHub [Issue](https://github.com/microsoft/vscode/issues/224581) that spawned the idea
* [Repository](https://github.com/RedCMD/JSON-Embedded-Languages)
* [Marketplace](https://marketplace.visualstudio.com/items?itemName=RedCMD.json-embedded-languages)


## TODO:
* `globs`/`"filenamePatterns"`
* Improve performance
