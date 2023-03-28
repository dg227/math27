# Python Code for MATH 27: Dynamical Systems with Applications

Tested with Python 3.11

## Virtual environment 

Create Python virtual environment:
```shell
python3 -m venv venv
```

Activate virtual environment:
```shell
source ./venv/bin/activate
```

Deactivate virtual environment:
```shell
deactivate
```

## Installation

1. The following packages may need to be installed on the system:
- nodejs
- pandoc
- pip
- yarn
- wheel

I used MacPorts on macOS to install these packages as follows:
```shell
port install nodejs18
port install pandoc
port install py-wheel
port install py-pip
port install yarn
```

2. Install `math27` package and dependencies by running the following command from within the `Python` directory:
```shell
pip install -e .
```

## Notebook output

Save notebook to HTML, including current state of widgets (check that Settings -> Save Widget State Automatically is selected):

```shell
jupyter nbconvert --to html --no-input <notebook_name>.ipynb
```

## Running from interpeter

```shell
import importlib as i
nl = i.import_module('nlsa')
i.reload(nl)
```

## Requirements metadata
To create requirements.txt:
```shell
pip freeze > requirements.txt
```
