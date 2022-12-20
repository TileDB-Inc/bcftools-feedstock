About bcftools
==============

Home: https://github.com/samtools/bcftools

Package license: GPL

Feedstock license: [BSD-3-Clause](https://github.com/TileDB-Inc/bcftools-feedstock/blob/main/LICENSE.txt)

Summary: BCFtools is a set of utilities that manipulate variant calls in the Variant Call Format (VCF) and its binary counterpart BCF. All commands work transparently with both VCFs and BCFs, both uncompressed and BGZF-compressed.  Most commands accept VCF, bgzipped VCF and BCF with filetype detected automatically even when streaming from a pipe. Indexed VCF and BCF will work in all situations. Un-indexed VCF and BCF and streams will work in most, but not all situations.

Current build status
====================


<table>
    
  <tr>
    <td>Azure</td>
    <td>
      <details>
        <summary>
          <a href="https://dev.azure.com/TileDB-Inc/feedstock-builds/_build/latest?definitionId=&branchName=main">
            <img src="https://dev.azure.com/TileDB-Inc/feedstock-builds/_apis/build/status/bcftools-feedstock?branchName=main">
          </a>
        </summary>
        <table>
          <thead><tr><th>Variant</th><th>Status</th></tr></thead>
          <tbody><tr>
              <td>linux_64</td>
              <td>
                <a href="https://dev.azure.com/TileDB-Inc/feedstock-builds/_build/latest?definitionId=&branchName=main">
                  <img src="https://dev.azure.com/TileDB-Inc/feedstock-builds/_apis/build/status/bcftools-feedstock?branchName=main&jobName=linux&configuration=linux%20linux_64_" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>osx_64</td>
              <td>
                <a href="https://dev.azure.com/TileDB-Inc/feedstock-builds/_build/latest?definitionId=&branchName=main">
                  <img src="https://dev.azure.com/TileDB-Inc/feedstock-builds/_apis/build/status/bcftools-feedstock?branchName=main&jobName=osx&configuration=osx%20osx_64_" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>win_64</td>
              <td>
                <a href="https://dev.azure.com/TileDB-Inc/feedstock-builds/_build/latest?definitionId=&branchName=main">
                  <img src="https://dev.azure.com/TileDB-Inc/feedstock-builds/_apis/build/status/bcftools-feedstock?branchName=main&jobName=win&configuration=win%20win_64_" alt="variant">
                </a>
              </td>
            </tr>
          </tbody>
        </table>
      </details>
    </td>
  </tr>
</table>

Current release info
====================

| Name | Downloads | Version | Platforms |
| --- | --- | --- | --- |
| [![Conda Recipe](https://img.shields.io/badge/recipe-bcftools-green.svg)](https://anaconda.org/tiledb/bcftools) | [![Conda Downloads](https://img.shields.io/conda/dn/tiledb/bcftools.svg)](https://anaconda.org/tiledb/bcftools) | [![Conda Version](https://img.shields.io/conda/vn/tiledb/bcftools.svg)](https://anaconda.org/tiledb/bcftools) | [![Conda Platforms](https://img.shields.io/conda/pn/tiledb/bcftools.svg)](https://anaconda.org/tiledb/bcftools) |

Installing bcftools
===================

Installing `bcftools` from the `tiledb` channel can be achieved by adding `tiledb` to your channels with:

```
conda config --add channels tiledb
conda config --set channel_priority strict
```

Once the `tiledb` channel has been enabled, `bcftools` can be installed with `conda`:

```
conda install bcftools
```

or with `mamba`:

```
mamba install bcftools
```

It is possible to list all of the versions of `bcftools` available on your platform with `conda`:

```
conda search bcftools --channel tiledb
```

or with `mamba`:

```
mamba search bcftools --channel tiledb
```

Alternatively, `mamba repoquery` may provide more information:

```
# Search all versions available on your platform:
mamba repoquery search bcftools --channel tiledb

# List packages depending on `bcftools`:
mamba repoquery whoneeds bcftools --channel tiledb

# List dependencies of `bcftools`:
mamba repoquery depends bcftools --channel tiledb
```




Updating bcftools-feedstock
===========================

If you would like to improve the bcftools recipe or build a new
package version, please fork this repository and submit a PR. Upon submission,
your changes will be run on the appropriate platforms to give the reviewer an
opportunity to confirm that the changes result in a successful build. Once
merged, the recipe will be re-built and uploaded automatically to the
`tiledb` channel, whereupon the built conda packages will be available for
everybody to install and use from the `tiledb` channel.
Note that all branches in the TileDB-Inc/bcftools-feedstock are
immediately built and any created packages are uploaded, so PRs should be based
on branches in forks and branches in the main repository should only be used to
build distinct package versions.

In order to produce a uniquely identifiable distribution:
 * If the version of a package **is not** being increased, please add or increase
   the [``build/number``](https://docs.conda.io/projects/conda-build/en/latest/resources/define-metadata.html#build-number-and-string).
 * If the version of a package **is** being increased, please remember to return
   the [``build/number``](https://docs.conda.io/projects/conda-build/en/latest/resources/define-metadata.html#build-number-and-string)
   back to 0.

Feedstock Maintainers
=====================


