1D and 2D barcode templating for spectroscopy
================
Philipp Baumann
; Update: 2019-11-26

# Overview

## Semi-automated barcode and label generation

## Fully automated barcode and label generation

To automate barcoding in python there are two packages,
[`python-barcode`](https://pypi.org/project/python-barcode/) for 1D and
[`qrcode`](https://pypi.org/project/qrcode/) for 2D Quick Response (QR)
codes. Both packages support exporting among others svg vector graphics
export.

# Details

There is many available barcode symbologies available. A symbology
represents both encoding of characters, quiet zone, start and stop
markers, as well as a check symbol (weighted sum of all symbols). Here
we chose the following symbologies:

  - 1D barcode: Code 128
  - 2D barcode: QR

Within Code 128, there are three code sets (A, B, C), which differ in
the 103 supported data symbols that are a subset of 128 ASCII
characters. Code sets A and B together support all ASCII characters,
whereas code set C is typically used to efficiently code digit strings.

## Raw label templates (pdf)

### Avery Zweckform L4778
