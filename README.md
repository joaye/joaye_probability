# joaye-probability package

This package consist of a set of python codes from Udacity AWS Machine Learning Foundations course where the goal is to deploy a package onto PyPi for Gaussian and Binomial Distribution.

# Background
## Gaussian Distribution
### Probability Density Function
![gaussian  pdf](https://github.com/joaye/joaye_probability/blob/master/img/gaussian_pdf.PNG)

## Binomial Distribution
### Binomial Mean
![binomial mean](https://github.com/joaye/joaye_probability/blob/master/img/binom_mean.PNG)
### Binomial Variance
![binomial mean](https://github.com/joaye/joaye_probability/blob/master/img/binom_variance.PNG)
### Binomial Standard Deviation
![binomial mean](https://github.com/joaye/joaye_probability/blob/master/img/binom_stdev.PNG)
### Probability Density Function
![binomial mean](https://github.com/joaye/joaye_probability/blob/master/img/binom_pdf.PNG)

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


