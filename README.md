# latexify

Short python script that creates a PNG image from a latex math expression.
It requires `latex` and `dvipng` to work. 

Example: `python latexify.py "y = \sum_{i=1}^n (w_i x_i) + b" -o example.png`

![program output](example.png)

# Usage

```
Usage: latexify.py [-h] [-v] [-o OUTPUTFN] [-d DPI] [--tempDir TEMPDIR]
                   expression

LaTeX to PNG utility

positional arguments:
  expression            Math expression to typeset in latex

optional arguments:
  -h, --help            show this help message and exit
  -v, --verbose         Show output from latex and dvipng commands
  -o OUTPUTFN, --outputFn OUTPUTFN
                        Output file name (will be a PNG file)
  -d DPI, --dpi DPI     DPI of output PNG
  --tempDir TEMPDIR     Directory where latex's intermediate files will be
                        written to
```