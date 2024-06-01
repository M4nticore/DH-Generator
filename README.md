# Diffie-Hellman Key Exchange and AES Encryption

This Python script demonstrates the Diffie-Hellman key exchange protocol combined with AES encryption for secure communication. 

## How it Works

1. **Generate DH Parameters**: Users input the DH parameters: `g` (generator), `p` (prime number), and their private keys.
2. **Generate Public Key**: The script calculates the public key based on the input private key and DH parameters.
3. **Generate Shared Secret**: Users input the other user's public key and generate a shared secret.
4. **Encryption**: The shared secret is hashed using SHA256 and used to derive an encryption key. The message is encrypted using AES in CBC mode with PKCS7 padding.
5. **Decryption**: The recipient decrypts the message using the same shared secret and AES decryption.

## Usage

1. Run the script.
2. Enter DH parameters when prompted.
3. Input the other user's public key.
4. Choose encryption or decryption.
5. Enter the message (for encryption) or ciphertext (for decryption) when prompted.

## Requirements

- Python 3.x
- pycryptodome library (`pip install pycryptodome`)
