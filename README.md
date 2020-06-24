# babelite
python-babel without support for Maltese language.

Babelite is the babel anaconda package with the mt.dat file removed.
It should behave the same as babel but without support for the Maltese language.

Babelite is setup as a local channel, so the install process consists of two steps.
1. First we have to tell conda about our new local channel and make sure it is the highest
   priority.  
2. Use conda to install babel as normal

	```
	conda config --prepend channels \path\whereyoudownloaded\babelite-master\local-channel
	conda install babel
	```


### Pin the version of babel

Probably not necessary, but if you want to ensure that a specific version is used I would recommend "pinning" the desired version of babel. For example the installation would look like the following:

	```
	conda config --prepend channels \path\whereyoudownloaded\babelite-master\local-channel
	conda install babel=2.7.0
	```
Create a file within the miniconda/conda-meta/ folder call "pinned" and within that folder insert text:

	```
	babel ==2.7.0
	```

Intended for use on Windows 10.
