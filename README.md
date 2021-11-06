# python-3.9.8-embed-amd64 with pip

*Working OS: Windows 10 64bit

This was made by following steps.

1. Download **[python-3.9.8-embed-amd64.zip](https://www.python.org/downloads/windows/)**
2. Download **[get-pip.py](https://bootstrap.pypa.io/get-pip.py)**
3. Run `python get-pip.py`
    ```plain
    $ python get-pip.py
    Collecting pip
    Downloading pip-21.3.1-py3-none-any.whl (1.7 MB)
        |████████████████████████████████| 1.7 MB 6.4 MB/s
    Collecting setuptools
    Downloading setuptools-58.5.3-py3-none-any.whl (946 kB)
        |████████████████████████████████| 946 kB ...
    Collecting wheel
    Using cached wheel-0.37.0-py2.py3-none-any.whl (35 kB)
    Installing collected packages: wheel, setuptools, pip

    WARNING: The script wheel.exe is installed in 'C:\******\python-3.9.8-embed-amd64\Scripts' which is not on PATH.
    Consider adding this directory to PATH or, if you prefer to suppress this warning, use --no-warn-script-location.
    WARNING: The scripts pip.exe, pip3.9.exe and pip3.exe are installed in 'C:\******\python-3.9.8-embed-amd64\Scripts' which is not on PATH.
    Consider adding this directory to PATH or, if you prefer to suppress this warning, use --no-warn-script-location.

    Successfully installed pip-21.3.1 setuptools-58.5.3 wheel-0.37.0
    ```
4. Edit `python39._pth` as...
   Before
   ```python
   #import site
   ```
   After
   ```python
   import site
   ```
5. Run `python -m pip --version`
   ```plain
   $ python -m pip --version
   pip 21.3.1 from C:\******\python-3.9.8-embed-amd64\lib\site-packages\pip (python 3.9)
   ```