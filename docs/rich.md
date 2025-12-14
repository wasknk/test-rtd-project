# rich 

## doc
https://rich.readthedocs.io/en/stable/


## Use with typer
```
import typer
from rich import print
app = typer.Typer()

data = {
    "name": "Rick",
    "age": 42,
    "items": [{"name": "Portal Gun"}, {"name": "Plumbus"}],
    "active": True,
    "affiliation": None,
}


@app.command()
def main():
    print("Here's the data")
    print(data)

if __name__ == "__main__":
    app()


```