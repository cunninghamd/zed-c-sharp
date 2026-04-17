# C# Syntax Highlighting for Zed

A [Zed](https://zed.dev) extension that adds C# language support with syntax highlighting, bracket matching, indentation, and code outline.

## Features

- Syntax highlighting via [tree-sitter-c-sharp](https://github.com/tree-sitter/tree-sitter-c-sharp)
- Bracket autoclosing and matching (`{}`, `[]`, `()`, `""`, `''`, `/* */`)
- Smart indentation
- Code outline (classes, methods, interfaces, etc.)
- String injection support
- File association: `.cs`
- Line comment shortcuts: `//` and `///`

## Installation

1. Clone this repository
2. Open Zed and go to the Extensions panel (`Cmd+Shift+X` / `Ctrl+Shift+X`)
2. Click `Install Dev Extension`
3. Choose the folder you cloned this repository to

### Installation Directly in your Zed Extensions

Clone this repository into your Zed extensions directory:

```sh
git clone https://github.com/cunninghamd/zed-c-sharp ~/.config/zed/extensions/zed-c-sharp
```

Then reload Zed or install via the Extensions panel pointing to the local path.

## Development

The extension uses Zed's extension schema v1. Grammar is pulled from the upstream [tree-sitter-c-sharp](https://github.com/tree-sitter/tree-sitter-c-sharp) grammar.

To work on highlight queries, edit `languages/csharp/highlights.scm` and reload the extension in Zed.
