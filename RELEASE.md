PyPi
====

Preparation:

* increment version in `setup.py`
* add new changelog section in `CHANGES.rst`
* ensure that help screens in `README.md` are up-to-date
* ensure that help screens on [hsi-website](https://github.com/wairas/hsi-website) are up-to-date
* commit/push all changes

Commands for releasing on pypi.org (requires twine >= 1.8.0):

```
find -name "*~" -delete
rm dist/*
python3 setup.py clean
python3 setup.py sdist
twine upload dist/*
```


Github
======

Steps:

* start new release (version: `vX.Y.Z`)
* enter release notes, i.e., significant changes since last release
* upload `happy_tools_tkinter-X.Y.Z.tar.gz` previously generated with `setup.py`
* publish


