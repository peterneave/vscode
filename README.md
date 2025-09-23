---
marp: true
theme: uncover
headingDivider: 3
paginate: true
---

<!--
_class:
 - lead
 - invert
-->

# Visual Studio Code <!--fit-->
<!-- _paginate: skip -->

Tips and Tricks

## Foreword
<!-- _paginate: skip -->

📝 Contribute on [![w:48](img/github-mark.svg) GitHub](https://github.com/peterneave/vscode)

🔗 View Online [neave.dev/vscode](https://neave.dev/vscode)

⬇️ Download [PowerPoint](https://neave.dev/vscode/vscode.pptx) and [PDF](https://neave.dev/vscode/vscode.pdf)

## What is VS Code?

> Visual Studio Code is a free code editor that is optimized for building and debugging modern web and cloud applications.

You can run it on Windows, Linux, Mac or Online <https://vscode.dev>

---

Key Features:

* It supports a range of languages,
* Productivity shortcut circuits
  - Keyboard shortcuts
  - Tasks
  - Snippets
* Customizable with
  - Themes
  - Extensions
* Integrated terminal.

## Documentation and Updates

- [Official Documentation](https://code.visualstudio.com/docs)
  - [Intro Videos](https://code.visualstudio.com/docs/getstarted/introvideos)
  - [Tips and Tricks](https://code.visualstudio.com/docs/getstarted/tips-and-tricks)
  - [Updates](https://code.visualstudio.com/updates)
- [VSCode YouTube Channel](https://www.youtube.com/@code)


## Inbuilt Features
<!-- footer: Inbuilt Features -->

### Help Menu

* [Keyboard shortcut reference](https://code.visualstudio.com/shortcuts/keyboard-shortcuts-windows.pdf)
* Walkthroughs
* Interactive Editor Playground
  - ![h:300px](img/tipsandtricks/editor-playground.jpg)

## Settings

### Profiles

![bg right:40% fit](img/tipsandtricks/create-profile.png)

VS Code has a Default Profile. You can have additional [profiles](https://code.visualstudio.com/docs/editor/profiles).

Customize Settings, Keyboard Shortcuts, User Snippets, User Tasks or  Extensions

---

- Have a profile for Frontend, Backend, AWS and Azure or even for a project.
- Customize the profile for a stack ie (Jira, AWS and Python).
- You could install the tools and extensions as part of that project.

## Customisation

- [Default settings](https://code.visualstudio.com/docs/getstarted/settings#_default-settings) or open `Preferences: Open Default Settings (JSON)`
- Customize it with User settings - `Ctrl+P` and go to `Open User Settings (JSON)`

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

### Synchronized Settings

![bg right h:300px](img/tipsandtricks/turn-on-sync.png)

[Settings sync](https://code.visualstudio.com/docs/editor/settings-sync) cross multiple instances of VS Code

## Layout

![w:800px](img/tipsandtricks/layout.png)

### Customize the layout

- You could move the sidebar to the right then when you `Toggle Sidebar/Ctrl+B` it doesn't make the code jump around.
- Add a secondary sidebar with Outline view for better navigation.

### Grouping

`Ctrl+\`

![bg right](img/tipsandtricks/split_editor.gif)

---

Switch to next group with `Ctrl+[1,2,3...]`

![w:1000px](img/tipsandtricks/navigate_editors.gif)

Alternatively: `Ctrl+P` and `View: Move Editor to Next Group`

## Navigation

`Ctrl+R` Displays a Quick Pick dropdown with the list from `File > Open Recent` with recently opened folders and workspaces followed by files.

### Multi-Root Workspaces

Normally your workspace has a single root/project folder but you can have a workspace with multiple project folders in Visual Studio Code with [multi-root workspaces](https://code.visualstudio.com/docs/editor/multi-root-workspaces). Uses a `.code-workspace` file

---

```json
{
  "folders": [
    {
      // Source code
      "name": "Product",
      "path": "vscode"
    },
    {
      // Docs and release notes
      "name": "Documentation",
      "path": "vscode-docs"
    },
    {
      // Yeoman extension generator
      "name": "Extension generator",
      "path": "vscode-generator-code"
    }
  ]
}
```

### Command Palette

![w:600px](img/tipsandtricks/OpenCommandPalatte.gif)
`Ctrl+Shift+P`

### Quick Open File

![w:600px](img/tipsandtricks/QuickOpen.gif)
`Ctrl+P`

---

![w:600px](img/tipsandtricks/quick-open-command-dropdown.png)

`Ctrl+P` and type `?term` to open a new terminal

### Sticky Scroll

See the code context with Sticky Scroll - useful for long methods

![w:600px](img/tipsandtricks/sticky-scroll.gif)

### Others

`Ctrl+T` - Go To Symbol
`Ctrl+G` - Go to Line
`Alt+ ← / →` - Jump forward and back

## Editing

### Text Manipulation

- Sort Lines Ascending/Descending
- Join Lines
- Transform Text

---

| Tranform | Example                  |
| -------: | :----------------------- |
|    Title | Hello World              |
|    Upper | HELLO WORLD              |
|    Lower | hello world              |
|    Camel | helloWorld               |
|    Snake | helloWorld → hello_world |
|    Kebab | helloWorld → hello-world |

### Code Formatting

![w:800px](img/tipsandtricks/code_formatting.gif)

### Regex Search and Replace

![w:800px](img/tipsandtricks/search_and_modify.png)

### Multi Cursor

Edit Text Vertically with [multi-cursor](https://code.visualstudio.com/docs/getstarted/tips-and-tricks#_multi-cursor-selection)

Keep selecting text with `Ctrl+D` and update over multiple locations in a file.

![w:800px](img/tipsandtricks/multicursor.gif)

### Expanding and Shrinking Selection

Shift+Alt+Left and Shift+Alt+Right

Great for finding the start and end of a long `<div>`

![](img/tipsandtricks/expandselection.gif)

### Folding

Hide Text for easier reading

![bg right w:500px](img/tipsandtricks/code_folding.gif)

Fold Level [1|2|3|4], Fold All, Unfold All

### Emmet

Generate HTML and CSS from shorthand. Works with multi-cursors

![bg left w:600px](img/tipsandtricks/emmet.gif)

### Markdown preview

![w:800px](img/tipsandtricks/md-dynamic-preview.gif)

## Productivity / Focus

### Zen Mode

Focus on the code with Zen Mode

![w:800px](img/tipsandtricks/zen_mode.gif)

### Errors

Jump to the [next error](https://code.visualstudio.com/Docs/editor/editingevolved#_errors-warnings) with `F8`

### File Nesting

[Nest](https://code.visualstudio.com/updates/v1_67#_explorer-file-nesting) related files under a parent file in the explorer.

![](img/tipsandtricks/file-nesting.jpg)

```json
"explorer.fileNesting.patterns": {
    "*.component.ts": "$(capture).component.html, $(capture).component.spec.ts, $(capture).component.scss",
    "README*": "AUTHORS,CHANGELOG*,CODE_OF_CONDUCT*,CONTRIBUTING*,LICENSE*"
  }
```

### Pinned Tabs

[Pinned Tabs](https://code.visualstudio.com/docs/editor/custom-layout#_pinned-tabs) allow you to keep a file open

![w:800px](img/tipsandtricks/pinned-editor-tab.png)

### Vertical Rulers

Make sure your code isn't getting too long and hard to read.

![w:800px](img/tipsandtricks/editor-rulers.png)

### LogPoints

Non-breaking [log points](https://code.visualstudio.com/blogs/2018/07/12/introducing-logpoints-and-auto-attach#_introducing-logpoints) to show logging

![w:800px](img/tipsandtricks/logpoints.gif)

### Screencast Mode

![w:600px](img/tipsandtricks/screencast.gif)

### Task Runners

Run tasks like build, test and other custom tasks in [Task Runners](https://code.visualstudio.com/docs/getstarted/tips-and-tricks#_task-runner).

![bg right w:500px](img/tipsandtricks/task_runner.gif)

### Remote Development

|                                                                                                                       Remote | Description                                                 |
| ---------------------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------- |
|                                                     [Remote via SSH](https://code.visualstudio.com/docs/remote/ssh-tutorial) | Connect to remote machines with Visual Studio Code via SSH. |
|                                                        [Work in WSL](https://code.visualstudio.com/docs/remote/wsl-tutorial) | Work in Windows Subsystem for Linux.                        |
|                                           [Develop in Containers](https://code.visualstudio.com/docs/devcontainers/tutorial) | Work in a Docker Container.                                 |
| [GitHub Codespaces](https://docs.github.com/github/developing-online-with-codespaces/using-codespaces-in-visual-studio-code) | Work in codespace with Visual Studio Code.                  |

---

#### Dev Containers

[Dev Containers](https://code.visualstudio.com/docs/devcontainers/containers) uses a `devcontainer.json` file in your project tells VS Code how to access (or create) a development container with a well-defined tool and runtime stack.

---

![](img/tipsandtricks/architecture-containers.png)

## Extensions
<!-- footer: Extensions -->

### Installation

Install extensions with `Ctrl+Shift+X`. You can add to the workspace `@recommended` extensions for a project.

[Most Popular](https://marketplace.visualstudio.com/search?target=VSCode&category=All%20categories&sortBy=Installs) extensions can be found with `@popular`

### Extension Packs

![bg content opacity:.2](img/extentions/extensionpacks.jpg)

[Extension Packs](https://marketplace.visualstudio.com/search?target=VSCode&category=Extension%20Packs&sortBy=Installs)

## Marp

This slide deck written in Markdown within VSCode. I used the Marp extension preview it. <https://marp.app/>

Marp has a CLI - so this slide has a CICD pipeline 😁

### Peacock

![bg right:50% w:500px](img/tipsandtricks/peacock.png)

[Peacock](https://marketplace.visualstudio.com/items?itemName=johnpapa.vscode-peacock) allows you to colour code VS Code.

### IntelliCode

AI-assisted development features for Python, TypeScript/JavaScript and Java developers

[IntelliCode](https://marketplace.visualstudio.com/items?itemName=VisualStudioExptTeam.vscodeintellicode)

![bg right w:500px](img/extentions/python-intellicode.gif)

### LiveServer

![bg left:50% w:600px](img/extentions/vscode-live-server-animated-demo.gif)

Launch a development local Server with live reload feature for static & dynamic pages

[LiveServer](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)

### Indent Rainbow

[Indent Rainbow](https://marketplace.visualstudio.com/items?itemName=oderwat.indent-rainbow)

![](img/extentions/indentrainbow.png)

### Path Intellisense

![bg left w:500px](img/extentions/pathintellisense.gif)

[Path Intellisense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.path-intellisense) autocompletes filenames


### Code Spell Checker

![bg right w:500px](img/extentions/codespellchecker.gif)

[Code Spell Checker](https://marketplace.visualstudio.com/items?itemName=streetsidesoftware.code-spell-checker) for source code

### LiveShare

Real-time collaborative development from the comfort of your favourite tools.

![bg left w:400px](img/extentions/liveshare.png)

[LiveShare](https://marketplace.visualstudio.com/items?itemName=MS-vsliveshare.vsliveshare) / [Docs](https://code.visualstudio.com/learn/collaboration/live-share)

### Jira and Bitbucket

Bringing the power of Jira and Bitbucket to VS Code

- You can create and view issues
- Start work on issues
- Create pull requests
- Do code reviews
- Start builds
- Get build statuses and more!

[Jira and Bitbucket](https://marketplace.visualstudio.com/items?itemName=Atlassian.atlascode)


### Error Lens

Improve highlighting of errors, warnings and other language diagnostics.

[Error Lens](https://marketplace.visualstudio.com/items?itemName=usernamehw.errorlens)

![](img/extentions/errorlens.png)

### Polacode

![bg right fit](img/extentions/polacode.gif)

📸  Polaroid for your code. Take screenshots of your code

[Polacode](https://marketplace.visualstudio.com/items?itemName=pnp.polacode)

### GitHub Copilot

[GitHub Copilot](https://marketplace.visualstudio.com/items?itemName=GitHub.copilot) Your AI pair programmer

![bg right w:800px](img/extentions/copilot.gif)

### C# Dev Kit

Official C# extension from Microsoft

- Project System / Solution Explorer
- Code Editing (Uses the C# extension)
- Package Management
- Debugging
- Testing

[C# Dev Kit](https://marketplace.visualstudio.com/items?itemName=ms-dotnettools.csdevkit)

### Polygot Notebooks

![bg left](img/extentions/polygot.png)

[Polygot Notebooks](https://marketplace.visualstudio.com/items?itemName=ms-dotnettools.dotnet-interactive-vscode) allows

C#, F#, PowerShell, JavaScript, SQL, KQL, Python, R, HTML, HTTP, Mermaid.

### API Clients

[REST Client](https://marketplace.visualstudio.com/items?itemName=humao.rest-client)

```http
GET https://example.com/topics/1 HTTP/1.1

POST https://example.com/comments HTTP/1.1
content-type: application/json

{
    "name": "sample",
    "time": "Wed, 21 Oct 2015 18:27:50 GMT"
}
```

```sh
curl https://www.google.com
```

---

![bg right fit](img/extentions/thunder-client-v2.png)

[Thunder Client](https://marketplace.visualstudio.com/items?itemName=rangav.vscode-thunder-client)

Lightweight Rest API Client for VS Code

### TODO Tree

[TODO Tree](https://marketplace.visualstudio.com/items?itemName=Gruntfuggly.todo-tree) quickly find all your todo items.

![bg left fit](img/extentions/todotree.png)

### Conventional Commits

![bg right:40% fit](img/extentions/conventionalcommits.gif)

```text
<type>[optional scope]: <description>

[optional body]

[optional footer(s)]
```

[Conventional Commits](https://marketplace.visualstudio.com/items?itemName=vivaxy.vscode-conventional-commits)
[conventionalcommits.org](https://www.conventionalcommits.org) which then dovetails to [semver.org](https://semver.org)

### Better Comments

![bg left fit](img/extentions/better-comments.png)

[Better Comments](https://marketplace.visualstudio.com/items?itemName=aaron-bond.better-comments) colour codes your commit messages

### Unique Lines

Keep [unique lines](https://marketplace.visualstudio.com/items?itemName=bibhasdn.unique-lines) of text and remove duplicates from current selection. Also includes a command to shuffle currently selected lines.

### Encode Decode

[Encode Decode](https://marketplace.visualstudio.com/items?itemName=mitchdenny.ecdc)

- Convert String **to/from** Base64, HTML Entities, JSON Byte Array, JSON String, Unicode, XML Entities
- Convert String to MD5/SHA1/SHA256/SHA512 (as Base64 or Hex)

### Bookmarks

![bg left fit](img/extentions/booksmarks.png)

[Bookmark](https://marketplace.visualstudio.com/items?itemName=alefragnani.Bookmarks) your code and quickly jump to bookmarks.

### Markdown Preview

![bg right:30%](img/extentions/mermaid.png)

[Markdown Preview](https://marketplace.visualstudio.com/items?itemName=bierner.markdown-mermaid) allows you to create [Mermaid JS](https://mermaid.js.org/) documents that can be included in Markdown documents.

```mermaid
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
```

---

Aside: Mermaid JS can generate

- Generate Flowchart
- Sequence Diagram
- Class Diagram
- State Diagram
- Entity Relationship Diagram
- User Journey
- Gantt
- Pie Chart
- Quadrant Chart
- Requirement Diagram

---

![bg right w:400px](img/extentions/mermaid-sequence.png)
![bg right w:400px](img/extentions/mermaid-flow.png)

```mermaid
sequenceDiagram
    Alice->>+John: Hello John, how are you?
    Alice->>+John: John, can you hear me?
    John-->>-Alice: Hi Alice, I can hear you!
    John-->>-Alice: I feel great!
```

```mermaid
flowchart TD
    A[Christmas] -->|Get money| B(Go shopping)
    B --> C{Let me think}
    C -->|One| D[Laptop]
    C -->|Two| E[iPhone]
    C -->|Three| F[fa:fa-car Car]
```

### JSON Crack

![bg left:60% fit](img/extentions/jsoncrack.gif)

[JSON Crack](https://marketplace.visualstudio.com/items?itemName=AykutSarac.jsoncrack-vscode) seamlessly visualize your JSON data instantly into graphs.

### SemanticDiff

![bg fit right:60%](img/extentions/semanticdiff.gif)

[SemanticDiff](https://marketplace.visualstudio.com/items?itemName=semanticdiff.semanticdiff) is a programming language aware diffs.

Can show differences when you move code.

### FootSteps

![bg fit left:60%](img/extentions/footsteps.gif)

[FootSteps](https://marketplace.visualstudio.com/items?itemName=Wattenberger.footsteps) Highlight and navigate between your most recently edited chunks of code

### Pets for your VS Code

![bg fit right:60%](img/extentions/pets.gif)

[Pets](https://marketplace.visualstudio.com/items?itemName=tonybaloney.vscode-pets) gives you a virtual pet to play with while you are coding.

### Docker

![bg right fit](img/extentions/docker-view-context-menu.gif)

Makes it easy to create, manage, and debug containerized applications.

[Docker](https://marketplace.visualstudio.com/items?itemName=ms-azuretools.vscode-docker)

### Azure Tools

![bg left fit](img/extentions/azure.png)
Get web site hosting, SQL and MongoDB data, Docker Containers, Serverless Functions and more, all on Azure.

[Azure Tools](https://marketplace.visualstudio.com/items?itemName=ms-vscode.vscode-node-azure-pack)

### AWS Toolkit

![bg right fit](img/extentions/aws.gif)

Including CodeWhisperer, CodeCatalyst, and support for Lambda, S3, CloudWatch Logs, and many other services

[AWS Toolkit](https://marketplace.visualstudio.com/items?itemName=AmazonWebServices.aws-toolkit-vscode)
