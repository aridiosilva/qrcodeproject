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


## Standards

There are several standards that cover the encoding of data as QR codes:

 - **October 1997 – AIM (Association for Automatic Identification and Mobility) International**
 - **January 1999 – JIS X 0510**
 - **June 2000 – ISO/IEC 18004:2000 Information technology** – Automatic identification and data capture techniques – Bar code symbology – QR code (now withdrawn) -
Defines QR code models 1 and 2 symbols.
 - **September 2006 – ISO/IEC 18004:2006 Information technology** – Automatic identification and data capture techniques – QR code 2005 bar code symbology specification (now withdrawn). Defines QR code 2005 symbols, an extension of QR code model 2. Does not specify how to read QR code model 1 symbols, or require this for compliance.
 - **February 2015 – ISO/IEC 18004:2015 Information** – Automatic identification and data capture techniques – QR Code barcode symbology specification Renames the QR Code 2005 symbol to QR Code and adds clarification to some procedures and minor corrections.

 At the application layer, there is some variation between most of the implementations. **Japan's NTT DoCoMo** has established de facto standards for the encoding of URLs, contact information, and several other data types. The **open-source "ZXing" project** maintains a list of QR code data types.

## Structure of a QR code (version 7)

Highlighting functional elements:

![Sctructure of QR Code](https://github.com/aridiosilva/qrcodeproject/blob/main/img/600px-QR_Code_Structure_Example_3.svg.png)

## Risks

The only context in which common QR codes can carry executable data is the URL data type. These URLs may host JavaScript code, which can be used to exploit vulnerabilities in applications on the host system, such as the reader, the web browser or the image viewer, since a reader will typically send the data to the application associated with the data type used by the QR code.

In the case of no software exploits, malicious QR codes combined with a permissive reader can still put a computer's contents and user's privacy at risk. This practice is known as "attagging", a portmanteau of "attack tagging".[94] They are easily created and can be affixed over legitimate QR codes.[95] On a smartphone, the reader's permissions may allow use of the camera, full Internet access, read/write contact data, GPS, read browser history, read/write local storage, and global system changes.

Risks include linking to dangerous web sites with browser exploits, enabling the microphone/camera/GPS, and then streaming those feeds to a remote server, analysis of sensitive data (passwords, files, contacts, transactions),[99] and sending email/SMS/IM messages or DDOS packets as part of a botnet, corrupting privacy settings, stealing identity,[100] and even containing malicious logic themselves such as JavaScript[101] or a virus. These actions could occur in the background while the user is only seeing the reader opening a seemingly harmless web page.[104] In Russia, a malicious QR code caused phones that scanned it to send premium texts at a fee of US$6 each.

-
