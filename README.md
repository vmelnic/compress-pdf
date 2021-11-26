# compress-pdf
Reduce the size of your PDF for easier sharing.

## Installation

Ghostscript is an interpreter for the PostScript® language and PDF files. https://www.ghostscript.com

```
brew install gs
```

## Usage

Run the following command:

```
gs -sDEVICE=pdfwrite -dCompatibilityLevel=1.4 -dPDFSETTINGS=/default -dColorImageResolution=150 -dNOPAUSE -dQUIET -dBATCH -sOutputFile="input.pdf" "output.pdf"
```

In order to have a beeto image quality, play with `ColorImageResolution` resolution:

```
-dColorImageResolution=150
```

More details are available here:

* https://www.ghostscript.com/doc/9.54.0/VectorDevices.htm#distillerparams
