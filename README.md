
# RSA Chat Application

This project implements a basic chat application using RSA encryption for secure communication. It includes three main components: RSA key generation and encryption/decryption, a client script, and a server script.

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
  - [RSA Key Generation and Encryption/Decryption](#rsa-key-generation-and-encryptiondecryption)
  - [Client Script](#client-script)
  - [Server Script](#server-script)
- [Contributors](#contributors)
- [License](#license)

## Introduction

The RSA Chat Application allows two users to securely communicate over a network using RSA encryption. The `client.py` script is used by the client to connect to a server, and the `server.py` script is used to host the server. Both client and server generate RSA key pairs to encrypt and decrypt messages.

## Features

- Secure communication using RSA encryption.
- Simple graphical user interface (GUI) for both client and server.
- Real-time message sending and receiving.
- Automatic RSA key pair generation.

## Requirements

- Python 3.x
- `sympy` library for prime number generation
- `tkinter` for the GUI

## Installation

1. Install Python 3 from the official [Python website](https://www.python.org/).
2. Install the `sympy` library using pip:

```sh
pip install sympy
```

## Usage

### RSA Key Generation and Encryption/Decryption

The `rsa.py` script includes functions to generate RSA key pairs, encrypt messages, and decrypt messages.

#### Functions

- `gcd(a, b)`: Calculates the greatest common divisor of `a` and `b`.
- `egcd(a, b)`: Performs the extended Euclidean algorithm.
- `mod_inverse(a, m)`: Calculates the modular inverse of `a` under modulo `m`.
- `isprime(n)`: Checks if a number `n` is prime.
- `generate_prime(bitlength)`: Generates a prime number of specified bit length.
- `generate_keypair(keysize)`: Generates RSA key pairs of specified key size.
- `encrypt(plain_text, package)`: Encrypts a plaintext message.
- `decrypt(msg_ciphertext, package)`: Decrypts a ciphertext message.

### Client Script

1. Run the client script:

```sh
python client.py
```

2. Enter your name in the console, server IP and port in the GUI.
3. Use the GUI to send and receive messages.

#### Code Overview

- Prompts the user to enter their name.
- Generates RSA key pairs.
- Connects to the server using the provided IP and port.
- Sends the public key to the server.
- Encrypts messages before sending them to the server.
- Decrypts received messages from the server.

### Server Script

1. Run the server script:

```sh
python server.py
```

2. Enter your name in the console, server IP and port in the GUI.
3. Use the GUI to send and receive messages.

#### Code Overview

- Prompts the user to enter their name.
- Generates RSA key pairs.
- Binds the server to the provided IP and port.
- Listens for incoming connections from clients.
- Sends the public key to the client.
- Encrypts messages before sending them to the client.
- Decrypts received messages from the client.

## Contributors

- [Erza Merovci](https://github.com/erzamerovci)
- [Ferdeze Nurkasa](https://github.com/FerdezeNurkasa)
- [Festim Krasniqi](https://github.com/FestimKrasniqi)

