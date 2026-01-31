# Image Steganography with AES Encryption
1. Introduction

This project implements a secure image steganography system using Least Significant Bit (LSB) technique combined with AES encryption. The application allows users to hide encrypted text inside an image and later extract and decrypt the hidden message using the correct secret key.

A Tkinter-based GUI is provided to make the encoding and decoding process simple and user-friendly.

2. Project Overview

Traditional steganography hides plain text inside images, which can be extracted if discovered. To enhance security, this project encrypts the message using AES (Advanced Encryption Standard) before embedding it into the image. Even if the hidden data is extracted, it remains unreadable without the correct encryption key.

3. Features

->Hide secret text inside images using LSB steganography
->AES encryption applied before embedding data
->Secure AES decryption during decoding
->Supports PNG, JPG, and JPEG images
->Simple and intuitive GUI using Tkinter
->Image quality preserved after encoding
->End-of-message marker to avoid garbage data during decoding

4. How It Works
#Encoding Process
->User selects an image.
->User enters a secret message.
->The message is encrypted using AES encryption.
->The encrypted text is converted to binary.
->Binary data is embedded into the least significant bits of image pixels.
->The encoded image is saved without visible distortion.

#Decoding Process
->User selects the encoded image.
->Hidden binary data is extracted from pixel values.
->The encrypted message is reconstructed.
->AES decryption is applied using the same secret key.
->Original message is displayed to the user.


! This project is intended for educational and research purposes to demonstrate secure data hiding techniques using cryptography and steganography.
