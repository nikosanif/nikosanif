# Curriculum Vitae

My curriculum vitae repository.

## Installation

- Install LaTeX

```sh
# macOS MacTex Install with homebrew
$ brew install mactex-no-gui --cask

# Arch Linux Family
$ sudo pacman -S texlive-most

# For Ubuntu, you might need a ppa:
$ sudo add-apt-repository ppa:jonathonf/texlive
$ sudo apt update && sudo apt install texlive-full

# Fedora
$ sudo dnf install texlive-scheme-full
```

- Update the packages

```sh
# macOS Updating the packages
$ sudo tlmgr update --self && sudo tlmgr update --all
```

- Install LaTeX Workshop plugin from the Visual Studio Code Marketplace

```sh
$ ext install latex-workshop
```

## Build project

- Use the following recipe at `settings.json`

```json
{
  // ...
  "latex-workshop.latex.recipes": [
    {
      "name": "latexmk (lualatex)",
      "tools": ["lualatexmk"]
    }
    // ...
  ]
}
```
