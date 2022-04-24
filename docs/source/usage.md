# Usage

## Installation

To use Lumache, first install it with `pip`:

```console
(.venv) $ pip install lumache
```

## Creating recipes

To retrieve a list of ingredients,
use the {py:func}`lumache.get_random_ingredients` function:

```{eval-rst}
.. autofunction:: lumache.get_random_ingredients
```

The `kind` parameter should be a {py:class}`str`,
otherwise the function will raise an exception:

```{eval-rst}
.. autoexception:: lumache.InvalidKindError
```