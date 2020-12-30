# Cryptography

Cryptography loosely translated means secret writing, and has been used for centuries with more and more advanced methods over time.

## Caesar cipher

A fairly simple cryptophraphy method, where each letter is advanced by some number so that when you input some letter, another letter is output. This allows for the sender of some message to encrypt their message, and the reciever to decrypt it, as long as each party knows the number.

## Enigma machines

Another quite famous example is the Enigma Machine used by the Nazis in WWII, cracked by Alan Turing and his team, who created their own vacuum tube computer to nearly automate the process.

Now, with the massive advances in computers, theses methods would not hold up, as a modern computer could try many many combinations very quickly to crack these algorithms.

## AES

AES or Advanced Encryption Standard is a modern take on encryption, where each party invents their own secret key, and mix that key with a public one to send to the other party. Each then mixes their own private key in a way that both parties end up with the same result, without ever having exposed their own private keys to the outside world.

You can then use your own private key plus the public key to encrypt data, and the other party can use their own private key plus the public key to decrypt it.

No encryption is 100% secure, and there is a tradeoff between performance (meaning the time it takes to encrypt and decrpyt some message) and security.

[<-- Back](../README.md)
