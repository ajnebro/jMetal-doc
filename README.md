# jMetal-doc
[![Read the Docs](https://img.shields.io/readthedocs/jmetal-doc.svg?style=flat-square)](https://readthedocs.org/projects/jmetal-doc/)

## Generate the docstring

First, make sure to have installed `javasphinx` and `recommonmark`:

```bash
pip install git+https://github.com/bronto/javasphinx.git recommonmark
```

Then, run:

```bash
javasphinx-apidoc -o docs/source/ --title='API' /path/to/jMetal
```