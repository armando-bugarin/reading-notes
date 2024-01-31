# Read: Class 18

1. **What is the basic principle behind the Caesar Cipher, and how was it used historically?**

Basic Principle: The Caesar Cipher is a substitution cipher where each letter in the plaintext is shifted a certain number of places down or up the alphabet. The shift is usually a fixed value known as the key.

Historical Use: Julius Caesar is often credited with using this cipher to communicate with his generals. However, it's not a highly secure encryption method, as there are only 25 possible keys (excluding the trivial case of a key of 0), making it susceptible to brute force attacks.

2. **What are the key differences between symmetric and asymmetric encryption? How is asymmetric used in secure communication today?**

Symmetric Encryption: In symmetric encryption, the same key is used for both encryption and decryption. It's faster and more efficient than asymmetric encryption but requires a secure way to share the secret key.

Asymmetric Encryption: Asymmetric encryption involves a pair of keys (public and private). The public key is used for encryption, and the private key is used for decryption. It provides a secure way to exchange keys over an insecure channel.

Secure Communication: Asymmetric encryption is often used in secure communication today for tasks like key exchange in protocols such as SSL/TLS. It allows secure communication between parties who may not have shared a secret key beforehand.

3. **How do computers generate random numbers, and what are the differences between true random number generation (TRNG) and pseudo-random number generation (PRNG)? Discuss their use cases in cryptography.**

Pseudo-Random Number Generation (PRNG): PRNGs use algorithms to generate sequences of numbers that appear random. They are deterministic and depend on an initial value called the seed. While useful for many applications, they are not truly random.

True Random Number Generation (TRNG): TRNGs generate random numbers from physical processes, like electronic noise or radioactive decay. They are considered truly random but can be slower and more expensive.

Use Cases in Cryptography: TRNGs are crucial for cryptographic applications where true randomness is essential (e.g., key generation). PRNGs are often suitable for non-cryptographic purposes, like simulations, where high speed and repeatability are more important than true randomness.

4. **What’s the difference between encryption and decryption? Explain with an analogy.**

Analogy: Imagine sending a confidential letter. Encryption is like putting the letter in a locked box (using a key), so only the person with the key can open it. Decryption is the process of unlocking the box using the correct key to reveal the original letter. In this analogy, the locked box is the encrypted message, the key is the encryption key, and the opened box is the decrypted message.

## `Things I want to know more about`
