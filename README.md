# `README.md` for [waa repo](https://github.com/Ai-Yukino/waa)

- Use a local python pip-installable module
- Imports from separate folders

---

## ❄ Instructions

Clone and navigate to the root of this repo, i.e. `/waa`. In your terminal, run

```
conda env create -f waa.yml
```

to install the provided conda virtual environment. Activate the environment with

```
conda activate waa
```

Next, run

```
pip install -e .
```

to `pip install` the provided `src` local python module. Finally, run

```
python waa.py
```

in your terminal to verify that the`src` module was successfully imported.

## 🌸 Note

The import statements in `waa/waa.py` are the main things to pay attention to. For example, in the second line of `waa.py`, we have

```
from src.uwu.msg import uwu
```

`src` is the name of a folder `waa/src` but also the package name specified in `waa/setup.py`. Next, `src.uwu` refers to the folder `src/uwu`, and `src.uwu.msg` refers to a python script `src/uwu/msg.py`. Lastly

```
... import uwu
```

refers to the function `uwu` defined inside of `src/uwu/msg.py`.

## ❄ References

- [Set up your project | goodresearch.dev](https://goodresearch.dev/setup.html)
