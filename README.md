# QR Code Project

## QR Code technology overview

The QR Code standard defines a method to encode a string of characters or bytes into a grid of black and white pixels. The text could be numbers, names, URLs, et cetera. Because the standard uses a 2D barcode, it can store much more information than a traditional 1D barcode. To illustrate for comparison, a 1D barcode usually stores 10 to 20 digits, while a QR code often stores 50 textual characters. Note that a QR Code barcode simply represents static data – the barcode does not inherently cause an action to be executed.

## Terminology

Some of the frequently used official terminology have non-intuitive meanings, as summarized below:

### QR Code

A popular international standard (symbology), created by Denso Wave, that specifies how messages are converted to barcodes.

### QR Code symbol

A single 2D graphical barcode, which results from the QR Code generation process. Informally this is called a “QR code” (without using the word symbol) or a barcode.

### Module

A black or white pixel in a QR Code symbol. Note that a module can be scaled to occupy multiple pixels on a screen or in an image file.

### Version

A way of measuring the size of a symbol, from 1 to 40. Version 1 has 21×21 modules, version 2 has 25×25, ..., and version 40 has 177×177. Note that all 40 versions are defined in a single standard, and this term differs from the conventional meaning of the word version.

### Model

Indicates the revision of the QR Code standard. (The word model here corresponds with the conventional meaning of the word version.) Model 1 QR codes are outdated and essentially never seen. Model 2 QR codes are widespread and dominant. Model 2 also has an extension called Micro QR codes (not implemented in my library). Note that model 1 defines versions 1 through 14, whereas model 2 QR defines versions 1 through 40, allowing much more data capacity.
