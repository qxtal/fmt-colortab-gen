# fmt-colortab-gen
Document generator script for the 'fmt Color Reference Table'.

This script generates a visual reference guide for the colors provided by [fmt](https://fmt.dev)'s color library in an HTML document. The values are extracted directly from `include/fmt/color.h` via the project's GitHub repository.

## Requirements
Python 3 and an active internet connection is all you need to run this.

## Usage
Download the `fmt_colortab_gen.py` script. Then run the script.

```bash
chmod +x fmt_colortab_gen.py
./fmt_colortab_gen.py
```

Alternatively (especially if running on Windows):

```bash
python fmt_colortab_gen.py
```

The script will download the `include/fmt/color.h` file from fmt's repository, filter the colors from the header file, and then generate an HTML file presenting the finalized color guide.

By default, it will save the document as `index.html` in the directory where the script is executed from. Custom filenames will be implemented in the next version.