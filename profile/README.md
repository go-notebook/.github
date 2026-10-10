<p align="center"><img src="https://raw.githubusercontent.com/go-notebook/brand/main/social/go-notebook.png" alt="go-notebook" width="720"></p>

# go-notebook

🌐 **[Website](https://go-notebook.github.io)** · 📚 **[Documentation](https://go-notebook.github.io/docs/)**

**Go notebooks with native speed, kept values and a reproducible order.**

A notebook is a Markdown file whose ` ```go ` blocks are cells. The kernel
compiles it into a real Go program, so cells run at native speed; orders the
cells by what they use, worked out from the code itself as marimo does for
Python, not by the order you ran them in; and runs only what changed. A cell
whose code and inputs did not change keeps its result, and its values are
handed over instead of being computed again, across rebuilds and across runs.

```sh
go install github.com/go-notebook/notebook/cmd/notebook@latest

notebook run analysis.md     # run it, print each cell's results
notebook html analysis.md    # run it, write analysis.html (no scripts, no external resources)
notebook watch analysis.md   # run it on every save and keep analysis.html current
```

## Repositories

| Repo | What it is |
|------|------------|
| [**notebook**](https://github.com/go-notebook/notebook) | the kernel, the `notebook` command and the HTML export (Go 1.27.2 or later) |
| [**docs**](https://github.com/go-notebook/docs) | the documentation site (Hugo + Hextra), served at [/docs/](https://go-notebook.github.io/docs/) |
| [**go-notebook.github.io**](https://github.com/go-notebook/go-notebook.github.io) | the landing page (Hugo) |
| [**brand**](https://github.com/go-notebook/brand) | logo, icons and social images |

It is part of an ecosystem with [go-ndarray](https://github.com/go-ndarray/ndarray)
(NumPy-style arrays) and [go-fft](https://github.com/go-fft/fft) (`numpy.fft`).
