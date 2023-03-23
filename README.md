# pywrap_example

## setup cmake
```
mkdir build && cd build
cmake ..
make mickey
make mickey_cpp
```

## setup bdist_wheel
```
python3 setup.py bdist_wheel
python3 -m venv .venv
./.venv/bin/pip install ./dist/cmake_example-0.0.1-cp38-cp38-linux_x86_64.whl
```
# Troubleshooting
## python error bdist_wheel
```
python3 -m pip install --upgrade setuptools pip
python3 -m pip install importlib

```

