# AES-128 Implementation in Python (ECB Mode)

## Overview

This Python script provides a complete implementation of the AES-128 encryption and decryption algorithm in Electronic Codebook (ECB) mode. The script reads input from text files, performs encryption or decryption based on user choice, and writes the output to other text files.

The AES algorithm is a symmetric key encryption standard widely used for securing sensitive data. It operates on fixed-size blocks of data and uses a key of 128, 192, or 256 bits. In this implementation, we focus on AES-128, which uses a 128-bit key.

## Files

- **keyExpansion.py**: Contains the function to expand the key for AES encryption.
- **AES_encryption.py**: Includes the encryption function for AES.
- **AES_decryption.py**: Includes the decryption function for AES.
- **display_manual.py**: Provides a function to display a manual for user guidance.
- **main.py**: The main script orchestrating key handling, encryption, and decryption operations.

## Usage

1. Ensure Python 3.x is installed on your system.
2. Place the plaintext in the file `plainText.txt`.
3. Place the original key in the file `original_key.txt`.
4. Run `main.py` to start the program.
5. Follow the on-screen instructions to perform encryption or decryption.

## Important Notes

- The implementation assumes input and output text files are encoded in UTF-8.
- ECB mode is used, which encrypts each block of plaintext independently. This can lead to certain security vulnerabilities and is not recommended for use in many scenarios.
- It is essential to handle keys securely and avoid hardcoding them in plaintext within scripts.

## Example

Suppose we have plaintext stored in `plainText.txt`:

```
Hello, world!
```

And the original key stored in `original_key.txt`:

```
thisisakeyforAES
```

After running the script and choosing encryption, the output cipher will be stored in `cipherText.txt`:

```
UÒþZÿÚ`Ii0ÒbG´
```

Decryption of this cipher will produce the original plaintext.
