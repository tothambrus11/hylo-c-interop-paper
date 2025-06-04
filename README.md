# LaTeX Research Paper

This repository contains a LaTeX research paper with automated building and deployment via GitHub Pages.

## Automated PDF Building

This project uses GitHub Actions to automatically compile the LaTeX document into a PDF whenever changes are pushed to the main branch. The compiled PDF is then published to GitHub Pages.

### How to Access the Latest PDF

The latest version of the PDF can be accessed at:
```
https://[your-github-username].github.io/[repository-name]/main.pdf
```

For example, if your GitHub username is "researcher" and the repository is named "research-paper", the URL would be:
```
https://researcher.github.io/research-paper/main.pdf
```

## Local Development

To build the PDF locally, you'll need a LaTeX distribution installed (such as TeX Live, MiKTeX, or MacTeX). Then you can compile the document using:

```
pdflatex main.tex
bibtex main
pdflatex main.tex
pdflatex main.tex
```

Alternatively, you can use a LaTeX editor like Overleaf, TeXStudio, or VS Code with LaTeX Workshop extension.

## Repository Structure

- `main.tex`: The main document file
- `sections/`: Contains individual sections of the paper
- `references.bib`: Bibliography file
- `.github/workflows/`: Contains GitHub Actions workflow for automated PDF building
