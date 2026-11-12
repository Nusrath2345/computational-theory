# Computational Theory

An implementation of the SHA-256 hash algorithm in Python and NumPy, built step by step from the [Secure Hash Standard (FIPS 180-4)](https://doi.org/10.6028/NIST.FIPS.180-4).

This repository is my submission for the Computational Theory module at ATU Galway


## Contents

| File | Purpose |
| --- | --- |
| `problems.ipynb` | The notebook containing all problems and their solutions. |
| `requirements.txt` | The Python packages needed to run the notebook. |
| `AGENTS.md` | Style instructions for AI coding assistants, supplied by the module lecturer. |

## Setup

These steps assume [Python 3](https://www.python.org/downloads/) and [git](https://git-scm.com/downloads) are installed.

1. Clone the repository:

   ```bash
   git clone https://github.com/Nusrath2345/computational-theory.git
   cd computational-theory
   ```

2. Install the required packages with [pip](https://pip.pypa.io/en/stable/user_guide/#requirements-files):

   ```bash
   pip install -r requirements.txt
   ```

3. Open the notebook with [Jupyter Notebook](https://jupyter-notebook.readthedocs.io/en/stable/):

   ```bash
   jupyter notebook problems.ipynb
   ```

4. In Jupyter, select **Kernel → Restart & Run All** to run every cell in order.

### Running in GitHub Codespaces

As an alternative to a local setup, open this repository on GitHub, select **Code → Codespaces → Create codespace on main**, then run step 2 in the Codespace terminal and open `problems.ipynb`. See the [GitHub Codespaces documentation](https://docs.github.com/en/codespaces/overview) for more detail.

## Tools and References

- [FIPS 180-4: Secure Hash Standard](https://doi.org/10.6028/NIST.FIPS.180-4): the official definition of SHA-256, which every problem is based on.
- [NumPy](https://numpy.org/doc/stable/): provides the fixed-width `uint32` integers used to represent 32-bit words.
- [NumPy data types](https://numpy.org/doc/stable/user/basics.types.html): explains `uint32` and how fixed-width integers overflow.
- [Python `hashlib`](https://docs.python.org/3/library/hashlib.html): Python's built-in SHA-256, used to test this implementation.
- [Python `bytes`](https://docs.python.org/3/library/stdtypes.html#bytes-objects): the type used for input messages.
- [Jupyter Notebook](https://jupyter.org/): the environment used to run `problems.
ipynb`.
- [Python `int.to_bytes` / `int.from_bytes`](https://docs.python.org/3/library/stdtypes.html#int.to_bytes): convert between integers and big-endian bytes.
- [NumPy byte order](https://numpy.org/doc/stable/user/basics.byteswapping.html): explains the `>` and `<` dtype prefixes used to read big-endian words.
- [Danny Cohen, *On Holy Wars and a Plea for Peace* (1980)](https://www.rfc-editor.org/ien/ien137.txt): the paper that introduced the terms big-endian and little-endian.

## Author

Nusrath