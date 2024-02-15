# O-RAN
Securing O-RAN Equipment Using Blockchain-based Supply Chain Verification
Verification of Cryptographic Firmware for Secure OpenRAN Devices

This code implements an example of how to use blockchain-based registration and cryptographic signatures to confirm the authenticity and integrity of firmware in OpenRAN equipment.

Important characteristics:

uses SHA-256 to calculate firmware hashes in order to verify their integrity.
uses the cryptography library to implement cryptographic signing and verification for safe authentication.
registers and verifies firmware hashes linked to equipment serial numbers using a virtual blockchain.
Application:

Configuration:

Replace "Vendor's public key" and "Vendor's private key" with the real PEM-formatted private and public keys.
Make sure you have pip install cryptography, the cryptography library, installed.
Processing of Firmware:

Make a firmware object and add a code and serial number to it.
Compute the firmware code's SHA-256 hash.
Initialization of Equipment:

Make an Equipment object by using the serial number.
