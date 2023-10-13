# {{ cookiecutter.package_name }}

This project uses:

{% if cookiecutter.build_tool == 'flit' %}* [flit](https://flit.pypa.io/en/stable/) for packaging{% endif -%}
{%- if cookiecutter.build_tool == 'poetry' %}* [poetry](https://python-poetry.org/) for dependency management{% endif %}
* [flake8](https://pypi.org/project/flake8/) for linting and
* [black](https://github.com/psf/black) for code formatting
* [isort](https://github.com/timothycrosley/isort) for import sorting

Development Tasks:

* Install dependencies: `make install`
* Run the test suite: `make test`
* Run lint checks: `make lint`
* Auto-format: `make format`
{% if cookiecutter.build_tool == 'flit' %}
Virtual Env Management:

* `source .venv/bin/activate`
* `deactivate`
{% endif %}