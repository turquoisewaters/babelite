# babelite
python-babel without support for Maltese language.

Babelite is the babel anaconda package with the mt.dat file removed.
It should behave the same as babel but without support for the Maltese language.

Babelite is setup as a local channel, so the install process is the same as usual except you have to
tell anaconda to use the local channel, where it is located, and the package you want to install.
This can be done using the --channel or -c option with conda install:

```
Examples...
conda install -c \path\whereyoudownloaded\your\babelite\folder babel
conda install -c \path\whereyoudownloaded\your\babelite\folder babel=2.8.0
conda install -c \path\whereyoudownloaded\your\babelite\folder babel=2.7.0
```


### Pin the version of babel
Probably optional, but for good measure I would recommend "pinning" the version of babel to the
one installed to help ensure that anaconda doesn't try to automatically update babel.

Create a file within the miniconda/conda-meta/ folder call "pinned" within that folder insert text:
```
babel ==2.8.0
or
babel ==2.7.0
```

Intended for use on Windows 10.
