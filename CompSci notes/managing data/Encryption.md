Encryption - "The process of encoding a message so it can be read only by the sender and the intended recipient"

Cipher - "replacing each letter with a different letter"

The Caesar cipher was an early form of encryption where each letter of the alphabet is shifted by a fixed distance

eg.
A B C D E F G
becomes
D E F G H I J

so the message FEED becomes IHHG

## Symmetric encryption

In symmetric encryption, a single key is used to both encrypt and decrypt a message
Both parties need to know the key and keep it secret
The same key can be used multiple times, or a unique key can be generated each time, for extra security
In symmetric encryption, there is a danger that the message can be cracked either by intercepting the key or duplicating the key
The security risk means that systems that receive or send sensitive information, like credit card details, use a more secure method of encryption known as asymmetric encryption

## Asymmetric encryption

In asymmetric encryption, the two parties use two different keys, starting with the unencrypted message that is encrypted with the first key
Once the message is encrypted and sent, the recipient decrypts the message with the second key
It is important that the key used by the sender is not the same as the key used by the receiver
It is almost impossible to determine one key with the other, making asymmetric encryption much more secure

The keys are generated in key pairs, meaning that anything encrypted with one key can be decrypted with its key pair
for asymmetric encryption to work, you need to pick one key from the key pair and make it the public key
the other becomes the private key

The public key can be accessed by anyone, but the private key is secure, and should not be sent to anyone

The public and private key are combined to create a combined encryption key

The combined encryption key is used to encrypt the message and send it

The public key is used to encrypt and the private key is used to decrypt