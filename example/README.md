# How to make and upload a python package to PyPi
## procedure
    pip install twine
    python setup.py sdist 
## upload the repository
### test PyPi  
You have to be registered on test.pypi.org first  

    twine upload --repository-url https://test.pypi.org/legacy/ dist/*
    pip install --index-url https://test.pypi.org/simple/ distributions

### PyPi  
You have to be registered on pypi.org first  

    twine upload dist/*
    pip install --index-url https://pypi.org/simple distributions
