# FastAPI Users - Database adapter for MongoDB

<p align="center">
  <img src="https://raw.githubusercontent.com/frankie567/fastapi-users/master/logo.svg?sanitize=true" alt="FastAPI Users">
</p>

<p align="center">
    <em>Ready-to-use and customizable users management for FastAPI</em>
</p>

[![build](https://github.com/fastapi-users/fastapi-users-db-mongodb/workflows/Build/badge.svg)](https://github.com/frankie567/fastapi-users/actions)
[![codecov](https://codecov.io/gh/fastapi-users/fastapi-users-db-mongodb/branch/master/graph/badge.svg)](https://codecov.io/gh/fastapi-users/fastapi-users-db-mongodb)
[![PyPI version](https://badge.fury.io/py/fastapi-users-db-mongodb.svg)](https://badge.fury.io/py/fastapi-users-db-mongodb)
[![Downloads](https://pepy.tech/badge/fastapi-users-db-mongodb)](https://pepy.tech/project/fastapi-users-db-mongodb)
<p align="center">
    <a href="https://www.buymeacoffee.com/frankie567"><img src="https://img.buymeacoffee.com/button-api/?text=Buy me a coffee&emoji=&slug=frankie567&button_colour=FF5F5F&font_colour=ffffff&font_family=Lato&outline_colour=000000&coffee_colour=FFDD00"></a>
</p>

---

**Documentation**: <a href="https://frankie567.github.io/fastapi-users/" target="_blank">https://frankie567.github.io/fastapi-users/</a>

**Source Code**: <a href="https://github.com/frankie567/fastapi-users" target="_blank">https://github.com/frankie567/fastapi-users</a>

---

Add quickly a registration and authentication system to your [FastAPI](https://fastapi.tiangolo.com/) project. **FastAPI Users** is designed to be as customizable and adaptable as possible.

**Sub-package for MongoDB support in FastAPI Users.**

## Development

### Setup environment

You should create a virtual environment and activate it:

```bash
python -m venv venv/
```

```bash
source venv/bin/activate
```

And then install the development dependencies:

```bash
pip install -r requirements.dev.txt
```

### Run unit tests

You can run all the tests with:

```bash
make test
```

The command will start a MongoDB container for the related unit tests. So you should have [Docker](https://www.docker.com/get-started) installed.

Alternatively, you can run `pytest` yourself:

```bash
pytest
```

There are quite a few unit tests, so you might run into ulimit issues where there are too many open file descriptors. You may be able to set a new, higher limit temporarily with:

```bash
ulimit -n 2048
```

### Format the code

Execute the following command to apply `isort` and `black` formatting:

```bash
make format
```

## License

This project is licensed under the terms of the MIT license.
