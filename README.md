# QR Code Project

## What does Mean QR CODE and its Origin

A QR code (abbreviated from Quick Response code) is a type of matrix barcode (or two-dimensional barcode) first designed in 1994 for the automotive industry in Japan.

A barcode is a machine-readable optical label that contains information about the item to which it is attached. In practice, QR codes often contain data for a locator, identifier, or tracker that points to a website or application.

A QR code uses four standardized encoding modes (numeric, alphanumeric, byte/binary, and kanji) to store data efficiently; extensions may also be used.

The Quick Response system became popular outside the automotive industry due to its fast readability and greater storage capacity compared to standard UPC barcodes. Applications include product tracking, item identification, time tracking, document management, and general marketing.

## History of QR

 - The QR code system was invented in 1994 by Masahiro Hara from the Japanese company Denso Wave.
 - The initial design was influenced by the black and white pieces on a Go board.
 - Its purpose was to track vehicles during manufacturing; it was designed to allow high-speed component scanning.
 - QR codes are now used in a much broader context, including both commercial tracking applications and convenience-oriented applications aimed at mobile-phone users (termed mobile tagging).
 - QR codes may be used to:

     - to display text to the user,
     - to open a webpage on the user's device,
     - to add a vCard contact to the user's device,
     - to open a Uniform Resource Identifier (URI),
     - to connect to a wireless network, or
     - to compose an email or text message.

 - There are a great many QR code generators available as software or as online tools that are either free, or require a paid subscription.
 - The QR code has become one of the most-used types of two-dimensional code.

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
