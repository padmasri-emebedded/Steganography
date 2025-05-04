Project Overview
This project implements steganography techniques to hide secret messages within image files using the Least Significant Bit (LSB) encoding method. By replacing the least significant bits of image data with bits of the secret message, information can be concealed within images without creating visible changes to the human eye.
Features

Encode Messages: Hide text messages within BMP image files
Decode Messages: Extract hidden messages from encoded images
Password Protection: Secure encoding/decoding with a secret key
Non-Destructive: Minimal visual impact on the carrier image
Command-Line Interface: Easy-to-use commands for encoding and decoding operations

Technologies Used

C Programming Language
File Operations
Pointers
Bitwise Operations
Functions
Makefiles
Command Line Arguments

How LSB Steganography Works
The Least Significant Bit (LSB) technique works by replacing the last bit of each byte in the image data with bits from the secret message:

The image is read byte by byte
For each byte, the least significant bit is replaced with a bit from the message
This causes minimal change to the color values (maximum change of 1)
These changes are imperceptible to the human eye
The message can later be extracted by reading the LSB of each byte

Key Learnings

Understanding image file structures and headers
Implementation of the LSB technique for information hiding
Working with binary file operations and bitwise manipulations
Developing a basic understanding of image processing concept
