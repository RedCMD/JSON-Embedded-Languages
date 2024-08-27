# JSON Embedded Languages

## Features

Syntax Highlighting for ShellScript language within `package.json` `"scripts"`
![Example `package.json` code](images/Example.png)


## Known Issues

ShellScript doesn't highlight code after `"`.  
Workaround is to place a `;` at the start of each string.  

This extension targets every JSON file, not just `package.json`.  
However only a root level `"scripts"` object is affected.  


---

## For more information

* The GitHub [Issue](https://github.com/microsoft/vscode/issues/224581) that spawned the idea
