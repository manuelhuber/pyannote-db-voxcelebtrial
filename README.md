# VoxCelebTrial
This is a simple db adapter that lists all files from the [trial pairs](http://www.robots.ox.ac.uk/~vgg/data/voxceleb/meta/veri_test.txt) as tst files. This DB does not contain train or development data. It is only used to generate features / embeddings etc. for the files. 

# pyannote.database plugin

This repository provides a template for creating your own [`pyannote.database`](http://github.com/pyannote/pyannote-database) plugin.

1. Fork this repository.
2. Edit `VoxCelebTrial/__init__.py`
3. Edit `setup.py`, `setup.cfg` and `.gitattributes`
4. Edit lines 45 to 48 in `VoxCelebTrial/_version.py`
5. Rename `VoxCelebTrial` directory to the name of your database (e.g. to [`Etape`](http://github.com/pyannote/pyannote-db-etape) or [`REPERE`](http://github.com/pyannote/pyannote-db-repere))
6. Commit and tag your changes using [`semantic versioning`](http://semver.org)
7. Run `pip install -e .` and enjoy!


In case your database is public and you want to share, I'd be happy to integrate your plugin in `pyannote`: a [pull request](https://help.github.com/articles/about-pull-requests/) to this repository should help us get started...
