# Man Page Syntax
VS Code extension providing simple language support for man page authoring, including syntax highlighting support, template pages as code snippets, and some other helpers.

## Features
The extension adds a `Man Page` language mode (file type). This can be manually selected when creating a new file, or will be auto-selected when opening man source files with the extension `.man`, `.mdoc` or a numbered page (`.1`-`.9`). 

### Man Page Language Mode
The language mode provides:
- Syntax highlighting
- Code snippets to create default page layouts with expected section headers
- Auto complete on some formatting instructions (e.g. `.nf`)

### Code Snippets
When creating a new page, it is important to maintain consistency with standard man page layouts.

Code snippets are used to provide some standard layouts for section headers for the various man page sections (e.g. 1 for user commands, 2 for system calls)

When creating a new man page, make sure the `Man Page` language mode is selected and then type `man` into the editor (or `man` followed by the number of the section page being created). A list of the available page templates will be displayed. Select the relevant one for the page being created - for example, `man1` is a code snippet that provides a template layout for a section 1 man page (user command). 

### Auto Complete
Certain man formatting commands require a start and end instruction, such as the `.nf`/`.fi` pair.

When using the Man Page language mode, typing the starting of one of these (e.g. `.nf`) will automatically insert the corresponding ending (e.g. `.fi`), either on the same or next line as appropriate.

## Known Issues
None at this time, but there may be some items not being highlighted and more standard page templates that could be presented as code snippets.

__Feedback is welcomed__ to allow this extension to grow and improve. Use the [issues](https://github.com/Motivesoft/vscode-man-page-syntax/issues) page for requests or to report bugs.

## Release Notes

### 1.0.0

- Improved syntax highlighting
- Template pages using code snippets
- Auto complete for formatting operations

### 0.0.2

- Improved syntax highlighting

### 0.0.1

- Initial release, basic syntax highlighting
