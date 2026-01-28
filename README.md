# The Agalmic Engine

## An Abundance Novel

In a future of technological abundance, this novel explores what happens when scarcity is largely solved. Drawing from economics, anthropology, and complexity science, it follows characters navigating the tensions that emerge when survival is no longer the primary driver of human behavior.

The story examines institutional design, human relationships, and the search for meaning in a world where material needs are met, but deeper questions about identity, purpose, and governance remain.

## Building the Manuscript

To generate a PDF for review:

**Prerequisites:**

*Windows:*
- Use WSL2 (see below) or go to the pandoc and miktex websites to get installation instructions.
- Pandoc: Install from [pandoc.org](https://pandoc.org/installing.html)
- LaTeX distribution: Install MiKTeX from [miktex.org](https://miktex.org/)

*Linux/WSL2 (Ubuntu/Debian):*
- Pandoc: `sudo apt update && sudo apt install pandoc`
- LaTeX distribution: `sudo apt install texlive-latex-base texlive-fonts-recommended texlive-extra-utils texlive-latex-recommended`

```bash
cd manuscript && xargs pandoc -o ../build/agalmic-engine.pdf --pdf-engine=pdflatex < chapters.txt
```

This creates a compiled PDF in the `build/` folder. Chapter order is defined in `manuscript/chapters.txt`.

**Adding or reordering chapters:**
1. Create the `.md` file in `manuscript/`
2. Add its filename to `chapters.txt` at the desired position

## Project Structure

- `manuscript/` - Individual chapter files in Markdown
- `manuscript/chapters.txt` - Chapter order manifest (used by build)
- `build/` - Compiled manuscripts (PDFs)
- `PREMISE.md` - Core vision and world-building principles
- `WORLD.md` - How the universe works
- `CHARACTERS.md` - Who acts and why
- `OUTLINE.md` - What is supposed to happen
- `agents.md` - Writing process framework

## Status

Work in progress. Feedback welcome!
