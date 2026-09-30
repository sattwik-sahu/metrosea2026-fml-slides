# Aether

*Lighter than Air, Clearer than Crystal*

A minimalist Beamer theme inspired by [SimplePlus](https://github.com/pm25/SimplePlus-BeamerTheme)

## Edit in Dev Container (zero setup)

New to LaTeX? You do not need to install anything except Docker and VS Code:

1. Install [Docker](https://docs.docker.com/get-docker/) and the [Dev Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers) extension for VS Code.
2. Open the `slides/` folder in VS Code.
3. Click **Reopen in Container** when VS Code offers it (first start downloads the TeX Live image, so grab a coffee).
4. Open [`main.tex`](./main.tex) and press `Ctrl+Alt+V` (or run **LaTeX Workshop: View LaTeX PDF**) to open the PDF next to the editor.
5. Edit any `.tex` file and save — the PDF rebuilds automatically and refreshes. `Ctrl+click` jumps between source and PDF (SyncTeX).

> The container ships full TeX Live + Biber and builds with the repo's [`.latexmkrc`](./.latexmkrc) (LuaLaTeX, output to [`build/`](./build/)), so what you see is exactly what CI/host builds produce.

## Quickstart Guide

1. Clone the repository
2. Update your slides title and subtitle in [`meta/commands.tex`](./meta/commands.tex)
3. Start adding `frame`s in files in the [`sections`](./sections/) directory, or create your own
  > Do not forget to add `\input{sections/your-file.tex}` in [`sections/index.tex`](./sections/index.tex) after creating them
4. Build [`main.tex`](./main.tex) with [LuaLatex](https://www.luatex.org/) to compile your slides into a PDF

## License

This project is released under the **Unlicense License**, granting you complete freedom to use, modify, and distribute the template. For more details, see the [LICENSE](./LICENSE) file.

