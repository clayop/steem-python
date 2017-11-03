# Official Python STEEM Library
`steem-python` is the official STEEM library for Python. It comes with a BIP38 encrypted wallet and a practical CLI utility called `steempy`.

## Preparation
You need to have `Python 3.6` or newer to install `steem-python`. Unfortunately, old Ubuntu versions do not support that version as a default so you need to install it manually. First, we can start with normal installation.

``` 
sudo apt-get update
sudo apt-get install -y python3-dev python3-pip build-essential libssl-dev libffi-dev
```

Then check Python version
```
python3 -V
```

If the version is lower than 3.6 (e.g. `Python 3.5.1`), you can try to install `Python 3.6` from the default repository.
```
sudo apt-get update
sudo apt-get install python3.6
```

If it fails, you can add a 3rd party repository and install.
```
sudo add-apt-repository ppa:jonathonf/python-3.6
sudo apt-get update
sudo apt-get install python3.6
```

The last step is replacing the default Python with the new one
```
rm /usr/bin/python
ln -s /usr/bin/python3.6 /usr/bin/python
```

After installation of `python3` and `pip3`, you need to install `pytest` by the following command.
```
pip3 install pytest
```


## Installation
You can install `steem-python` with `pip`:

```
pip3 install -U steem
```

## Documentation
Documentation is available at **http://steem.readthedocs.io**

## TODO
* more unit-tests
* 100% documentation coverage

## Notice
This library is under *active development*. Use at own discretion.

