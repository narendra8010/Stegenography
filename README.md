# Image Steganography using LSB Encoding and Decoding

## Overview
This project implements Image Steganography using the Least Significant Bit (LSB) technique in C. It hides a secret text file inside a BMP image without visibly changing the image. The hidden message can later be extracted using the decoding module.

## Features
- Encode a secret text file into a BMP image
- Decode the hidden message from the stego image
- Uses Least Significant Bit (LSB) encoding
- Supports BMP image format
- Command-line interface
- File handling and bitwise operations

## Technologies Used
- C Programming
- File Handling
- Bitwise Operations
- Structures
- Modular Programming

## Project Structure
- `main.c` – Main driver program
- `encode.c` – Encoding implementation
- `decode.c` – Decoding implementation
- `common.h` – Common declarations
- `encode.h` – Encoder definitions
- `decode.h` – Decoder definitions
- `types.h` – Data type definitions

## How to Compile

```bash
gcc *.c -o stego
```

## Run

### Encode

```bash
./stego -e beautiful.bmp secret.txt stego.bmp
```

### Decode

```bash
./stego -d stego.bmp output.txt
```
