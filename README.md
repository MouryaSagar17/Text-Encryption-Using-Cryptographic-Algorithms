# Text-Encryption-Using-Cryptographic-Algorithms
We can build a simple web application to encrypt and decrypt textual information that the user keys in. Remember that strong encryption should produce different outputs even given the same input.

Author : Mourya 

+ [Introduction](#intro)
+ [Requirements](#Requirements)
+ [Explanation](#Explain)
+ [Execution](#Execute)




# Introduction <a name="intro"> 
1. Objective: Implement text encryption and decryption using the AES-256-CBC algorithm in Node.js, ensuring data security and integrity.
2. Importance: Securely encrypting text data is essential for protecting sensitive information from unauthorized access and ensuring privacy.
# Requirements <a name="Requirements">
1. Node.js and npm: Ensure you have Node.js and npm (Node Package Manager) installed on your system.
2. You can download and install them from Node.js official website.
3. Dependencies:
   1. crypto: This module is part of the Node.js standard library, so no additional installation is required for it.
   2. dotenv: This module is used to load environment variables from a .env file into process.env.
# Explanation <a name="Explain"> 
1. Environment Variables: The encryption key is stored in an environment variable for security purposes. Ensure you have a .env file with the following content:
```javascript
ENCRYPTION_KEY=your-32-character-long-key
```
2. IV_LENGTH: The length of the Initialization Vector (IV) is set to 16 bytes, as required by the AES-256-CBC algorithm.

**Encryption Function:** 
1. Generates a random IV.
2. Creates a Cipher instance with the AES-256-CBC algorithm, the encryption key, and the IV.
3. Encrypts the input text and concatenates the encrypted data with the IV.

**Decryption Function:**
1. Splits the input text to extract the IV and encrypted data.
2. Creates a Decipher instance with the AES-256-CBC algorithm, the encryption key, and the IV.
3. Decrypts the encrypted data to retrieve the original text.

# Execution and Output: <a name="Execute"> 
  1. Run test.js file


     ![proof for text Encryption execution](https://github.com/MouryaSagar17/Text-Encryption-Using-Cryptographic-Algorithms/assets/143429477/240e6b7f-3b11-4f16-98a2-c53cb27e6665)



