# Cryptography

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.8+-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/Cryptography-Fernet-2F855A?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Status-Educational-1F6FEB?style=for-the-badge"/>
</p>

A lightweight Python project demonstrating **Fernet-based symmetric encryption** using the `cryptography` library. The repository focuses on the core workflow of generating a secure key and using it to decrypt encrypted files, making it a good starting point for understanding modern encryption in Python.

---

## Why this project?

Instead of relying on complex cryptography frameworks, this project keeps the implementation simple and readable while using **Fernet**, which provides authenticated AES encryption out of the box.

It demonstrates:

* Secure key generation
* Symmetric encryption concepts
* File decryption using a Fernet key
* Clean and beginner-friendly Python code

---

## Repository Structure

```text
Cryptography/
├── GenerateKey.py      # Generates and stores a Fernet key
├── DecryptFile.py      # Decrypts encrypted files using the key
└── README.md
```

---

## Getting Started

### Requirements

* Python 3.8 or later
* `cryptography` package

Install the dependency:

```bash
pip install cryptography
```

---

## Usage

### Step 1 — Generate a Key

Run:

```bash
python GenerateKey.py
```

A file named `encryption_key.txt` will be created containing a newly generated Fernet key.

### Step 2 — Configure the Decryption Script

Open `DecryptFile.py` and replace the placeholder with your generated key.

```python
key = b"YOUR_GENERATED_KEY_HERE"
```

### Step 3 — Decrypt Files

Run:

```bash
python DecryptFile.py
```

The script reads the configured encrypted files, decrypts them using the Fernet key, and writes the recovered content into `decryption.txt`.

---

## How Fernet Works

Fernet is built on modern cryptographic standards and provides:

* AES-based symmetric encryption
* Built-in authentication to detect tampering
* URL-safe encoded keys
* Secure random key generation

Because encryption and decryption use the same secret key, protecting the generated key is essential.

---

## Notes

* Keep `encryption_key.txt` private.
* Only decrypt files encrypted with the matching Fernet key.
* The current implementation is intentionally minimal to highlight the encryption workflow.

---

## Disclaimer

This repository is intended for **educational purposes** and should only be used on files and systems you own or have explicit authorization to work with.

---

## Author

**Shivam Sharma**

Cybersecurity • Python • Automation

* GitHub: **@fakcodr**
* YouTube: **FakCodr**
* Instagram: **@fakcodr**
