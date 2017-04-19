# Introduction

A presentation on computing persistent homology using javaplex.

# View Presentation

View the presentation [here](https://elliot2560.github.io/BasicPersistentHomologyPresentation/index.html).  Use arrow keys to navigate. Hit `s` key to view speaker notes. Hit `f` key to view slides in full screen.

# Installation

You can install the repository locally by 
```
git clone --recursive git://github.com/Elliot2560/BasicPersistentHomologyPresentation
```

# Run

View the slides locally by simply opening the `slides.html` file in a browser (preferably chrome/chromium or firefox).

# Conversion

With the following command, you can convert the .md file to the reveal.js slides using pandoc
```
pandoc -f markdown_github+yaml_metadata_block+tex_math_dollars+link_attributes+native_divs -t revealjs --mathjax --standalone slides.md -o slides.html -S -V theme=\"solarized\" --slide-level=2 -c custom.css -A mathjax_settings.html -M date=\"`date \"+%B %e, %Y\"`\"
```

If you wish to turn the presentation into a self contained html file without external dependencies, you can change the `--standalone` option to `--self-contained`.
