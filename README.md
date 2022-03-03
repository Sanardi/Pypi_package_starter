# Example Package

This is a simple example package. You can use
[Github-flavored Markdown](https://guides.github.com/features/mastering-markdown/)
to write your content.

To publish a package:

python3 -m pip install --upgrade pip

python3 -m pip install --upgrade build

python3 -m build

python3 -m pip install --upgrade twine

python3 -m twine upload --repository testpypi dist/*


generate a Token on your Pypi acount and when prompted use username "__token__"

as the password use the full token including the pypi prefix



to install your own package use:

python3 -m pip install --index-url https://test.pypi.org/simple/ --no-deps example-package-YOUR-USERNAME-HERE

then you can use in your script:

from example_package import example

example.add_one(2)