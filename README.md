# Homepage for lecture "Simulation Software Engineering"

This repository contains the content of for the homepage of the "Simulation Software Engineering" lecture and University of Stuttgart (Germany). The homepage is built on [mkdocs](https://www.mkdocs.org), the ["Material for MkDocs" theme](https://squidfunk.github.io/mkdocs-material/), and corresponding plugins.


## Structure of the repository

- `mkdocs.yml`: MkDocs configuration file
- `docs/`: The directory contains the Markdown files for the different pages of the homepage.
- `.github/workflows/ci.yml`: Definition file of GitHub action which builds the homepage on every successfull push.
- `README.md`: The Readme file you are currently reading

## Build homepage

**Dependencies**

- [Python 3](https://www.python.org/)
- [MkDocs](https://www.mkdocs.org)
- [Material for MkDocs theme](https://squidfunk.github.io/mkdocs-material/)
- [Pygments](https://pygments.org/)
- [Python Markdown Extensions](https://facelessuser.github.io/pymdown-extensions/)

The tools used are all based on Python 3 so the easiest way to install the theme and all dependencies is to use [pip](https://pypi.org/project/pip/). Running

```bash
pip install mkdocs-material
```

will install the MkDocs, theme, and the plugins.

If you use an operating system with  `pip` point

Alternative ways of building the homepage using MkDocs and Material for MkDocs are described in the [documentation of the theme](https://squidfunk.github.io/mkdocs-material/getting-started/).

**Building the homepage locally**

After installing all dependencies change into this directory (the directory containing the file named `mkdocs.yml`) and run `mkdocs serve`. This will start a local webserver on `127.0.0.1:8000`. Type in this address in a browser to see the local version of the homepage. While `mkdocs serve` is running it will monitor the files for changes and rebuild the homepage as needed.