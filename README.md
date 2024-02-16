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
--------------------------------------------------------------------------------------------------
Project Name: OpenRAN Equipment Node Initialization with Blockchain Verification

Description:

This Python program implements the Equipment Node Initialization process described in Section III.D of a paper discussing blockchain-based security for OpenRAN equipment.
It simulates connecting to a Quorum blockchain and sending a serial number and firmware hash for verification using a smart contract.

Purpose:

This code serves as a demonstration of the core flow for verifying equipment authenticity and integrity in OpenRAN networks using blockchain technology. 
It showcases how Python libraries like web3.py can interact with a permissioned blockchain like Quorum.

Requirements:

Python 3.6+
web3.py library (install with pip install web3)
Access to a Quorum blockchain network and deployed smart contract (not included in this code)

Replace placeholders:
Update quorum_provider with your Quorum node RPC endpoint.
Replace contract_address with the actual address of your deployed smart contract.
Modify YOUR_PRIVATE_KEY with your private key for interacting with the contract.
Ensure the verifyEquipment function call matches your contract's arguments and return values.
Run the program:
Execute python openran_equipment_verifiaction_web3.py.
Observe output:
The program will simulate sending a transaction with the equipment data and wait for confirmation.
It will then print a message indicating successful verification or potential issues.
