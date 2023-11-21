<!--
theme: gaia
headingDivider: 2
paginate: true
-->

<!--
_class:
 - lead
 - invert
-->

# Visual Studio Code
<!-- _paginate: skip -->

Tips and Tricks

## Foreword
<!-- _paginate: skip -->

This presentation is open source and available on [Github](https://github.com/peterneave/vscode).

You can view this presentation at [![w:48](img/github-mark-white.svg) GitHub](https://github.com/peterneave/vscode)

🔗[neave.dev/vscode](https://neave.dev/vscode), [PowerPoint](https://neave.dev/vscode/vscode.pptx) and [PDF](https://neave.dev/vscode/vscode.pptx)

## Documentation and Updates

https://www.youtube.com/@code

https://code.visualstudio.com/docs
https://code.visualstudio.com/docs/getstarted/introvideos
https://code.visualstudio.com/docs/getstarted/tips-and-tricks

https://code.visualstudio.com/updates

## Inbuilt Features

* Help Menu
  * [Keyboard Shortcut reference](https://code.visualstudio.com/shortcuts/keyboard-shortcuts-windows.pdf)
  * Walkthroughs
  * Command Palette CTRL+SHIFT+P
* Demo Mode
* Navigate between recently opened files and workspaces <kbd>Ctrl+R</kbd>
* Next Problem in Files <kbd>F8</kbd>
* Profiles
* Synchronized Settings
* Tunnelling Remote Explorer
* Terminal
* Grouping
* Duplicate Lines
* Expanding and Shrinking Selection
* Multi Cursor (CTRL+D)
* Sidebar and secondary sidebar with outline view
* Zen Mode
* Vertical Bars
* Code Formatting
* Folding
* Markdown preview
* Log Points
* Task Runners

## Customisation

Settings.json

```json
{
  "editor.fontFamily": "'Cascadia Code'",
  "editor.formatOnSave": true,
  "editor.rulers": [ 120 ],
  "editor.stickyScroll.enabled": true,
  "editor.trimAutoWhitespace": true,
  "explorer.fileNesting.enabled": true,
  "files.trimTrailingWhitespace": true,
  "git.branchPrefix": "yourusername/",
  "terminal.integrated.fontFamily": "'CaskaydiaCove Nerd Font Mono','Cascadia Code',Consolas,'Courier New',monospace",
  "workbench.sideBar.location": "right"
}
```

 File Nesting - See https://www.youtube.com/shorts/5kikdSqDm48

## Extensions

## Marp

This slide deck written in Markdown within VSCode. I used the Marp extension to export to PowerPoint. <https://marp.app/>

Side note, Marp has a CLI - so this slide has a CICD pipeline 😁

---

## Others

* CoPilot
* Atlassian
* Azure
* AWS
* Docker
* Developer Containers
* Error Lens
* Polacode
* Polygot Notebooks
* Rapid Clients
* Rest Client
* Presentations
* To Do Tree
* Unique Lines
* Sort
* Decode
* Bookmark
* Mermaid JS
* JSON Crack
* SemDiff
* FootSteps
* VS Code Pets - https://marketplace.visualstudio.com/items?itemName=tonybaloney.vscode-pets
