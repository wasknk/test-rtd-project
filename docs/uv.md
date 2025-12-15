# uv

## install 

```
pip install uv
# or 
pipx install uv

```

## Usage 

```bash
## create venv
uv venv
## activate venv
source .venv/bin/activate
## install all the dependencies and delete ones that are not in the list
uv sync
```

## See what installed
```
uv pip list
```

 
## Just generate a requirements.txt for CI/CD

```
uv pip compile pyproject.toml -o requirements.txt
```


## build 
```
uv build .
```