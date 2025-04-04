# Doc2txt-antiword

## Overview

**Antiword Converter** is a Python package designed to convert Microsoft Word `.doc` files into plain text format using the [Antiword](https://www.softpedia.com/get/Office-tools/Other-Office-Tools/Antiword.shtml) binary. This package provides a simple interface for converting `.doc` files to `.txt` format, either returning the converted text or writing it to an output file.

### Features:

- Converts `.doc` files to plain `.txt` format.
- Uses the **Antiword** binary for high-accuracy extraction.
- Simple API for converting documents with just one function.
- Error handling for common issues like missing files or incorrect formats.

## Requirements

- Python 3.6+
- Antiword binary (included in the package)

## Installation

To install `doc2txt-antiword` python package using `pip:`

`pip install doc2txt-antiword`

[pypi.org](https://pypi.org/project/doc2txt-antiword/ "https://pypi.org/project/doc2txt-antiword/")

To install the **doc2txt-antiword** package, follow these steps:

1. Clone the repository:

   ```bash
   git clone https://github.com/Bhola-straive/doc2txt-antiword.git
   ```
2. Navigate into the directory:

   ```bash
   cd doc2txt-antiword
   ```
3. Install the package using `pip`:

   ```bash
   pip install .
   ```

   This will install the `doc2txt-antiword` package and its dependencies.

## Usage

Once installed, you can use the `AntiwordConverter` class to convert `.doc` files into `.txt` format.

### Example: Converting a `.doc` File and Returning the Text

```python
 from doc2txt.converter import AntiwordConverter

# Initialize the converter
converter = AntiwordConverter()

# Path to the input .doc file
doc_path = '/path/to/your/document.doc'

# Convert the .doc file to text and print the result
converted_text = converter.convert_doc_to_txt(doc_path)

if converted_text:
    print("Converted Text:")
    print(converted_text)
else:  # converted_text is None
    print("Conversion failed.")
```
