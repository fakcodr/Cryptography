# Cryptography

A simple Python project demonstrating **symmetric encryption and decryption** using the `cryptography` library's **Fernet** implementation.

> **Educational Purpose:** This project is intended to demonstrate how Fernet encryption works for securely encrypting and decrypting files.

## Features

* Generate a secure Fernet encryption key
* Save the generated key to a file
* Decrypt encrypted files using the stored key
* Beginner-friendly Python implementation

## Project Structure

```text
Cryptography/
├── GenerateKey.py    # Generates and saves a Fernet key
├── DecryptFile.py    # Decrypts encrypted files using the key
└── README.md
```

## Requirements

* Python 3.8+
* `cryptography` library

Install dependencies:

```bash
pip install cryptography
```

## Usage

### 1. Generate an Encryption Key

Run:

```bash
python GenerateKey.py
```

This creates:

```text
encryption_key.txt
```

which contains the generated Fernet key.

### 2. Configure the Key

In `DecryptFile.py`, replace the empty key value with the generated key from `encryption_key.txt`.

Example:

```python
key = b"YOUR_GENERATED_KEY_HERE"
```

### 3. Decrypt Files

Run:

```bash
python DecryptFile.py
```

The script reads the encrypted files listed in the program, decrypts them using the Fernet key, and writes the decrypted output to:

```text
decryption.txt
```

## How Fernet Works

Fernet provides:

* AES encryption
* Authentication to prevent tampering
* Secure random key generation
* Simple API for encryption and decryption

## Disclaimer

This repository is for **educational and learning purposes only**. Only use these scripts on files you own or have explicit permission to work with.

## Author

**Shivam Sharma**

* GitHub: https://github.com/fakcodr
* YouTube: https://www.youtube.com/@fakcodr
* Instagram: https://www.instagram.com/fakcodr
