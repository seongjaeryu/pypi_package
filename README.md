# Python Packaging Projects

## Instruction

### Prerequisite
- `pip install twine`

### Prepare upload
1. `cd <package_folder>`
1. `python setup.py sdist`

### Upload test package to pypi test repository
- `twine upload --repository-url https://test.pypi.org/legacy/ dist/*`
- To install uploaded test package:
	- `pip install --index-url https://test.pypi.org/simple/ <package_name>`

### Upload package to pypi repository
- `twine upload dist/*`
- To install uploaded test package:
	- `pip install <package_name>`

> `pypi.org` and `test.pypi.org` need separate accounts.

## Reference
- https://packaging.python.org/tutorials/packaging-projects/
- [distutils](https://docs.python.org/3/distutils/) (Distributing Python Modules)

## Template
- /package

## Working on it
- /seongjaeryu
