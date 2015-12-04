<!-- README.md is generated from README.Rmd. Please edit that file -->
Some experiments in using raw HTML in R help files. Basically, raw HTML can be placed inside `\html{}` macros in `.Rd` files and **roxygen2** comments.

To see an example, install via `devtools::install_github('noamross/htmlhelp` and run `?hello`.

See `man/macros/macros.Rd` and `R/macros.R` for how it works.

Assets to be used in the HTML should be placed in the `inst/doc` directory. When referring to these files, it should be like so: `<img src="../doc/myfile.png">`.

Right now the raw HTML shows up in other help file formats. You may want to use the `\if{html}` macro to avoid this.

I'm not sure where this will lead. It emerged out a discussion of how to get feedback on documentation, so the thought was to put a feedback form at the bottom of help files. One could also include images, such as example plots (à la [**staticdocs**](https://github.com/hadley/staticdocs).

Please fork, PR, comment in the issues, do whatever you want with this, etc. I'd love to see your experiments
