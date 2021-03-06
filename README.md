# legos.ctftime

[![Travis](https://img.shields.io/travis/bbriggs/legos.ctftime.svg)](https://travis-ci.org/bbriggs/legos.ctftime) [![PyPI](https://img.shields.io/pypi/pyversions/legos.ctftime.svg)](https://pypi.python.org/pypi/legos.ctftime) [![PyPI](https://img.shields.io/pypi/v/legos.ctftime.svg)](https://pypi.python.org/pypi/legos.ctftime) [![PyPI](https://img.shields.io/pypi/wheel/legos.ctftime.svg)](https://pypi.python.org/pypi/legos.ctftime) [![PyPI](https://img.shields.io/pypi/l/legos.ctftime.svg)](https://pypi.python.org/pypi/legos.ctftime) [![PyPI](https://img.shields.io/pypi/status/legos.ctftime.svg)](https://pypi.python.org/pypi/legos.ctftime)

Interact with CTFtime API via chat to find out information about upcoming CTF events, team rankings, and more.

## Usage

## Installation

`pip3 install legos.ctftime`

This is a Lego designed for use with [Legobot](https://github.com/bbriggs/Legobot), so you'll get Legobot along with this. To deploy it, import the package and add it to the active legos like so:

```python
# This is the legobot stuff
from Legobot import Lego
# This is your lego
from legos.ctftime import CTFtime

# Legobot stuff here
lock = threading.Lock()
baseplate = Lego.start(None, lock)
baseplate_proxy = baseplate.proxy()

# Add your lego
baseplate_proxy.add_child(CTFtime)
```

## Tweaking

While you can use this one as-is, you could also add a localized version to your Legobot deployment by grabbing [ctftime.py](legos/ctftime.py) and deploying is as a local module. [Example of a Legobot instance with local modules](https://github.com/voxpupuli/thevoxfox/)

## Contributing

As always, pull requests are welcome.

