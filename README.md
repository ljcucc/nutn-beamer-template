# How to write & build beamer slides on macOS

If you have written briefings in markdown, or have LLM generate some markdown slides,
you can use this method to produce high-quality slides.

## Installation

You must install [Homebrew](https://brew.sh)

```sh
# for markdown to beamer
brew install pandoc

# for latex
brew install tectonic
```

## Markdown to beamer latex

```sh
pandoc -t beamer -i /path/to/doc.md -o ./src/index.tex
```

## Build pdf document

```sh
tectonic -X build --open
```
