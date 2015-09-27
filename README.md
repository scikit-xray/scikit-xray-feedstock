About conda-forge
-----------------

Conda forge is a GitHub organization containing a collection of repositories,
with each repository representing a single conda recipe. Each repository has
continuous integration enabled to automatically build (where appropriate) on
Linux, Windows and OSX through the gracious offerings of CircleCI, Appveyor
and TravisCI respectively.

To manage the continuous integration, and ensure that each of the respective
configurations are consistent across each of the recipe repositories
[conda-smithy](http://github.com/conda-forge/conda-smithy) has a collection of
tools for automatically generating the circle.yml, appveyor.yml and .travis.yml
based on the ci_config.yml within this repository.


Terminology
-----------

**feedstock** - the conda recipe (raw material)
**conda-smithy** - the tool which helps orchestrate the recipe/feedstock.
                   Its primary use is in the construction of the CI .yml files.
**conda-forge** - the place where the feedstock and smithy live and work to
                  produce the finished article (built conda distributions)


Updating scikit-xray-feedstock
------------------------------

TODO

Add binstar token to travis.yml
-------------------------------

```
gem install travis
travis encrypt BINSTAR_TOKEN={{ token }} -r github-organization/github-repo --add env.matrix
```
