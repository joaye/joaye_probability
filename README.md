# joaye-probability package

This package consist of a set of python codes from Udacity AWS Machine Learning Foundations course.

# Files

 setup.py\
 joaye_probability\
 &nbsp;&nbsp;&nbsp;├──__init.py\
 &nbsp;&nbsp;&nbsp;├──Binomialdistribution.py\
 &nbsp;&nbsp;&nbsp;├──Gaussiandistribution.py\
 &nbsp;&nbsp;&nbsp;└──Generaldistribution.py

# Installation
To download package:
`pip install joaye-probability`

To upload onto pypi
```cd binomial_package_files

# .tar.gz file: source archive
# python3 setup.py sdist bdist_wheel
# .whl file: built distribution
python setup.py sdist
pip install twine

# commands to upload to the pypi test repository
twine upload --repository-url https://test.pypi.org/legacy/ dist/*
pip install --index-url https://test.pypi.org/simple/ dsnd-probability

# command to upload to the pypi repository
twine upload dist/*
pip install dsnd-probability


