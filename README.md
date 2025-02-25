## gitsummary

Pure python utility to print a one-line summary of the current git repository, the current branch, and the hash for the current head.

### Installation

``` shell
pip install gitsummary
```
or
``` shell
conda -c conda-forge install gitsummary
```

### Usage

``` python
import gitsummary
gitsummary.print_cwd_git_version()
```


returns a string containing the current git repository, the current branch, and the hash of the branch head.  This information is useful in scientific codes to quickly determine the origin of a plot or dataset.  The string can, for example, be written in a [jupyter notebook](https://jupyter.org/) or placed in the metadata of a [netcdf](https://www.unidata.ucar.edu/software/netcdf/) file.  

The git repository is reported as final portion of the URL of the remote 'origin'.  If there is no remote named origin, it uses the full path on disk to the .git directory.   

## License

This project is licensed under the terms of the MIT license.
