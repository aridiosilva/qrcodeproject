# QR Code Project

This project aims to be Code to genenrate QR Codes.

## More Info

- [Wikipedia: QR code](https://en.wikipedia.org/wiki/QR_code)
- [QRcode.com by Denso Wave](https://www.qrcode.com/en/)
- [ISO/IEC 18004:2006 – QR Code 2005 bar code symbology specification (recommended)](https://web.archive.org/web/20140630004133/https://www.codeplex.com/Download?ProjectName=qrcodenet&DownloadId=321409)
- [ISO/IEC 18004:2000 – Bar code symbology – QR Code (old standard)](https://web.archive.org/web/20140630152807/http://www.codeplex.com/Download?ProjectName=qrcodenet&DownloadId=284291)
- [Thonky.com: QR Code Tutorial](https://www.thonky.com/qr-code-tutorial/)

## Additional Info to browse

- [Creating a QR Code step by step](https://www.nayuki.io/page/creating-a-qr-code-step-by-step)
- [Optimal text segmentation for QR Codes](https://www.nayuki.io/page/optimal-text-segmentation-for-qr-codes)
- [Fast QR Code generator library](https://www.nayuki.io/page/fast-qr-code-generator-library)
- [1D barcode generator (JavaScript)](https://www.nayuki.io/page/1d-barcode-generator-javascript)
- [Absolute and relative lens apertures](https://www.nayuki.io/page/absolute-and-relative-lens-apertures)

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
 - **[September 2006 – ISO/IEC 18004:2006 Information technology](http://www.iso.org/iso/iso_catalogue/catalogue_tc/catalogue_detail.htm?csnumber=43655)** – Automatic identification and data capture techniques – QR code 2005 bar code symbology specification (now withdrawn). Defines QR code 2005 symbols, an extension of QR code model 2. Does not specify how to read QR code model 1 symbols, or require this for compliance.
 - **[February 2015 – ISO/IEC 18004:2015 Information](https://www.iso.org/standard/62021.html)** – Automatic identification and data capture techniques – QR Code barcode symbology specification Renames the QR Code 2005 symbol to QR Code and adds clarification to some procedures and minor corrections.

 At the application layer, there is some variation between most of the implementations. **Japan's NTT DoCoMo** has established de facto standards for the encoding of URLs, contact information, and several other data types. The **open-source "ZXing" project** maintains a list of QR code data types.

## Structure of a QR code (version 7)

Highlighting functional elements:

![Sctructure of QR Code](https://github.com/aridiosilva/qrcodeproject/blob/main/img/600px-QR_Code_Structure_Example_3.svg.png)

## Risks

The only context in which common QR codes can carry executable data is the URL data type. These URLs may host JavaScript code, which can be used to exploit vulnerabilities in applications on the host system, such as the reader, the web browser or the image viewer, since a reader will typically send the data to the application associated with the data type used by the QR code.

In the case of no software exploits, malicious QR codes combined with a permissive reader can still put a computer's contents and user's privacy at risk. This practice is known as "attagging", a portmanteau of "attack tagging". They are easily created and can be affixed over legitimate QR codes. On a smartphone, the reader's permissions may allow use of the camera, full Internet access, read/write contact data, GPS, read browser history, read/write local storage, and global system changes.

Risks include linking to dangerous web sites with browser exploits, enabling the microphone/camera/GPS, and then streaming those feeds to a remote server, analysis of sensitive data (passwords, files, contacts, transactions), and sending email/SMS/IM messages or DDOS packets as part of a botnet, corrupting privacy settings, stealing identity, and even containing malicious logic themselves such as JavaScript or a virus. These actions could occur in the background while the user is only seeing the reader opening a seemingly harmless web page. In Russia, a malicious QR code caused phones that scanned it to send premium texts at a fee of US$6 each.

# Design

Unlike the older, one-dimensional barcodes that were designed to be mechanically scanned by a narrow beam of light, a QR code is detected by a 2-dimensional digital image sensor and then digitally analyzed by a programmed processor. The processor locates the three distinctive squares at the corners of the QR code image, using a smaller square (or multiple squares) near the fourth corner to normalize the image for size, orientation, and angle of viewing. The small dots throughout the QR code are then converted to binary numbers and validated with an error-correcting algorithm.

## (1) Storage

The amount of data that can be stored in the QR code symbol depends on the datatype (mode, or input character set), version (1, ..., 40, indicating the overall dimensions of the symbol, i.e. 4 × version number + 17 dots on each side), and error correction level. The maximum storage capacities occur for version 40 and error correction level L (low), denoted by 40-L:[7][65]

## (2) Error correction

QR Code has error correction capability to restore data if the code is dirty or damaged.

Four error correction levels are available for users to choose according to the operating environment. Raising this level improves error correction capability but also increases the amount of data QR Code size.

- Level L (Low)	7% of data bytes can be restored.
- Level M (Medium)	15% of data bytes can be restored.
- Level Q (Quartile)[66]	25% of data bytes can be restored.
- Level H (High)	30% of data bytes can be restored.

To select error correction level, various factors such as the operating environment and QR Code size need to be considered. Level Q or H may be selected for factory environment where QR Code get dirty, whereas Level L may be selected for clean environment with the large amount of data. Typically, Level M (15%) is most frequently selected.

The QR Code error correction feature is implemented by adding a Reed-Solomon Code to the original data.

The error correction capability depends on the amount of data to be corrected. For example, if there are 100 codewords of QR Code to be encoded,50 of which need to be corrected, 100 codewords of Reed-Solomon Code are required, as Reed-Solomon Code requires twice the amount of codewords to be corrected. In this case, the total codewords are 200, 50 of which can be corrected. Thus, the error correction rate for the total codewords is 25%. This corresponds to QR Code error correction Level Q.

In the example above, the error correction rate for QR Code codewords can be considered as 50%. However, it is not always the case that codewords of not Reed-Solomon Code but only QR Code are susceptible to dirt and damage.QR Code therefore represents its error correction rate as a ratio of the total codewords.

When discussing the Reed–Solomon code phase there is some risk for confusion, in that the QR ISO standard uses the term codeword for the elements of F256, which respect to the Reed–Solomon code are symbols, whereas it uses the term block for what with respect to the Reed–Solomon code are the codewords. The number of data versus error correction bytes within each block depends on (i) the version (side length) of the QR symbol and (ii) the error correction level, of which there are four. The higher the error correction level, the less storage capacity. The following table lists the approximate error correction capability at each of the four levels:

In larger QR symbols, the message is broken up into several Reed–Solomon code blocks. The block size is chosen so that no attempt is made at correcting more than 15 errors per block; this limits the complexity of the decoding algorithm. The code blocks are then interleaved together, making it less likely that localized damage to a QR symbol will overwhelm the capacity of any single block.

Due to error correction, it is possible to create artistic QR codes that still scan correctly, but contain intentional errors to make them more readable or attractive to the human eye, as well as to incorporate colors, logos, and other features into the QR code block.

It is also possible to design artistic QR codes without reducing the error correction capacity by manipulating the underlying mathematical constructs. Also uses of image processing algorithms are used to reduce errors in QR-code.

## (3) Encoding

The format information records two things: the error correction level and the mask pattern used for the symbol. Masking is used to break up patterns in the data area that might confuse a scanner, such as large blank areas or misleading features that look like the locator marks. The mask patterns are defined on a grid that is repeated as necessary to cover the whole symbol. Modules corresponding to the dark areas of the mask are inverted. The format information is protected from errors with a BCH code, and two complete copies are included in each QR symbol.

The message dataset is placed from right to left in a zigzag pattern, as shown below. In larger symbols, this is complicated by the presence of the alignment patterns and the use of multiple interleaved error-correction blocks.

![](https://github.com/aridiosilva/qrcodeproject/blob/main/img/420px-QR_Format_Information.svg.png)


Meaning of format information. In the above figure, the format information is protected by a (15,5) BCH code, which can correct up to 3 bit errors. The total length of the code is 15 bits, of which 5 are data bits (2 EC level + 3 mask pattern) and 10 are extra bits for error correction. The format mask for these 15 bits is: [101011001010101]. Note that we map the masked values directly to its meaning here

![](https://github.com/aridiosilva/qrcodeproject/blob/main/img/420px-QR_Character_Placement.svg.png)

Message placement within a QR symbol. The message is encoded using a (255,249) Reed Solomon code (shortened to (24,18) code by using "padding") which can correct up to 3 byte errors.

![](https://github.com/aridiosilva/qrcodeproject/blob/main/img/420px-QR_Ver3_Codeword_Ordering.svg.png)

Larger symbol illustrating interleaved blocks. The message has 26 data bytes and is encoded using two Reed-Solomon code blocks. Each block is a (255,233) Reed Solomon code (shortened to (35,13) code), which can correct up to 11 byte errors in a single burst, containing 13 data bytes and 22 "parity" bytes appended to the data bytes. The two 35-byte Reed-Solomon code blocks are interleaved so it can correct up to 22 byte errors in a single burst (resulting in a total of 70 code bytes). The symbol achieves level H error correction

The general structure of a QR encoding is as a sequence of 4 bit indicators with payload length dependent on the indicator mode (e.g. byte encoding payload length is dependent on the first byte).

The general structure of a QR encoding is as a sequence of 4 bit indicators with payload length dependent on the indicator mode (e.g. byte encoding payload length is dependent on the first byte).

![](https://github.com/aridiosilva/qrcodeproject/blob/main/img/generic_structure_qr_code_mode_indicator.jpg)

Four-bit indicators are used to select the encoding mode and convey other information.

![](https://github.com/aridiosilva/qrcodeproject/blob/main/img/generic_structure_qr_code_econding_modes.jpg)

Encoding modes can be mixed as needed within a QR symbol. (e.g., a url with a long string of alphanumeric characters )

```
[ Mode Indicator][ Mode bitstream ] --> [ Mode Indicator][ Mode bitstream ] --> etc... --> [ 0000 End of message (Terminator) ]
```

After every indicator that selects an encoding mode is a length field that tells how many characters are encoded in that mode. The number of bits in the length field depends on the encoding and the symbol version.

![](https://github.com/aridiosilva/qrcodeproject/blob/main/img

  Alphanumeric encoding mode stores a message more compactly than the byte mode can, but cannot store lower-case letters and has only a limited selection of punctuation marks, which are sufficient for rudimentary web addresses. Two characters are coded in an 11-bit value by this formula:

  ```
  V = 45 × C1 + C2
  ```

  This has the exception that the last character in an alphanumeric string with an odd length is read as a 6-bit value instead.

  ![](https://github.com/aridiosilva/qrcodeproject/blob/main/img/generic_structure_qr_code_alphanumeric_char_codes.jpg)








