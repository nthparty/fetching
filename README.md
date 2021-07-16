# fetching

Python tool for automatically wrapping multiple (possibly private) Python libraries \
into a single portable module file.

## purpose

This tool can be used to automatically extract files from multiple repositories and \
package them into a single portable module file.

## installation and usage

The package is available on PyPi:

```shell
python -m pip install fetching
```

The library can be imported as follows:

```python
from fetching import Fetching
```

Fetching relies on the GitHub API, and as such won't work unless you either pass a valid \
token to the `fetch_and_build()` method, or store one in either the `GH_TOKEN` or `GITHUB_TOKEN` \
environment variables.

## testing

Running `test.py` relies on either the `GH_TOKEN` or `GITHUB_TOKEN` environment variables \
being set.