# mkapi-fix

A fork of mkapi with a couple of _fixes_ that fit my use

Note that those _fixes_ may not make sense for your case

## Install
```bash
pip install mkapi-fix
# make sure you only have mkapi either or mkapi-fix installed
```

## Fixes/Modifications

- Fix when module prefix is None
- Skip `__wrapped__` check if errored
- Fix when decorators return the same object
- Fix when `annotations.__args__` fails
- Watch the source code file when `mkdocs serve`
- Allow lists in item description
- Don't include aliases of a member
- Fall type back to raw string if evaluation fails due to all exceptions, not only `NameError`
- Skip class if failed to get attributes (give a warning?)
- Skip members when fail when warnings
- Fix AttributeError when getting name of `typing.Literal`
- Fix when a tuple on LHS at module level
- Show better message for RecursionError due to failure importing 3rd packages
