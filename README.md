# cookiecutter-python-package

A cookiecutter template for creating an empty python package just how I like it.

## Publishing

The generated project contains a PyPI publish workflow using the [Trusted Publisher](https://docs.pypi.org/trusted-publishers/) model.
This requires two additional setup steps before it can be used:

1. Create a pending publisher in PyPI: https://docs.pypi.org/trusted-publishers/creating-a-project-through-oidc/
2. Create an environment called "publish" in GitHub: https://docs.github.com/en/actions/deployment/targeting-different-environments/using-environments-for-deployment#creating-an-environment
