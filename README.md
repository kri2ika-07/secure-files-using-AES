# secure-files-using-AES
my final project for Elevate Labs
# Secure File Storage System using AES Encryption

A beginner-friendly Python project that securely encrypts and stores files using AES-based encryption (Fernet). Also generates metadata with a hash and timestamp for file integrity.

## Objective
Create a secure local system for encrypting user files and storing verification data (hash, timestamp) using Python.

## Tech Stack
- Python 3.10+
- cryptography (Fernet)
- hashlib
- JSON
- CLI (Command Line)

## Folder Structure
SecureFileStorageAES/
├── generate_key.py # Creates encryption key
├── encrypt_file.py # Encrypts file + stores metadata
├── mykey.key # Secret AES key (excluded from Git)
├── metadata.json # File name + hash + timestamp
├── encrypted_files/ # Stores .enc files
│ └── test.txt.enc


##  How It Works

1. Run `generate_key.py` → creates `mykey.key`
2. Run `encrypt_file.py` → encrypts input file
3. Saves `.enc` file in `encrypted_files/`
4. Logs metadata to `metadata.json` with hash & timestamp

## Example Metadata

json
{
  "file_name": "test.txt",
  "encrypted_file": "encrypted_files/test.txt.enc",
  "timestamp": "2025-06-27T21:12:00",
  "hash": "fcbb87bcb2748c137..."
}
## What I Learned
  Real-world use of AES (via Fernet)
  Hashing with SHA-256
  python file I/O + JSON
  Basics of cryptography


## Future Features
  Decryption with password
  GUI with Tkinter
  Key management & backup




