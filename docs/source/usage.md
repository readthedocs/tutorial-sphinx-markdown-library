# Usage

## Installation

To install Lumache:

```console
(.venv) $ pip install lumache
```

## Creating recipes

To create a recipe, you can use the {py:func}`lumache.get_random_ingredients` function:

```{eval-rst}
.. autofunction:: lumache.get_random_ingredients
```

Sometimes, an {py:exc}`lumache.InvalidKindError` will be raised:

```{eval-rst}
.. autoexception:: lumache.InvalidKindError
```