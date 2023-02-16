Installing python: [](https://realpython.com/installing-python/)[https://realpython.com/installing-python/](https://realpython.com/installing-python/)

Installing pip:

```bash
python3 -m pip install --user --upgrade pip

python3 -m pip --version
```

Installing virtualenv:

```bash
python3 -m pip install --user virtualenv
```

Creating a virtual environment:

```bash
# Creating at local folder:
python3 -m venv env_name
```

Activate/deactivate environment:

```bash
# Activate:
source env_name/bin/activate

# Deactivate:
deactivate
```

Installing packages:
```bash
python3 -m pip install package_name

# From requirements.txt:
python3 -m pip install -r requirements.txt
```
