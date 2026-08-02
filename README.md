# public-key-to-address
Convert an EVM public key to an address
---------------------------------------------------
This library will calculate ethereum address from a public key.

The script calculates an EVM address based on a public key: it takes the provided key, removes the service prefix 0x04, processes the resulting data using the Keccak-256 cryptographic hashing algorithm, discards the first 12 bytes of the resulting hash, and keeps the final 20 bytes, applying the EIP-55 algorithm—a checksum that converts individual letters of the address to uppercase based on the hash of the address itself to protect the user from errors caused by manual entry or copying.

**For Windows**

Step 1. Press Win+R

![Image alt](https://github.com/Gene-stack/public-key-to-address/blob/main/img1.jpg)

Step 2. Paste the command and click OK

After that, the cmd will open. You need to enter the public key so that an EVM wallet can be calculated from it.

![Image alt](https://github.com/Gene-stack/public-key-to-address/blob/main/img2.jpg)

Step 3. Input your public key and press Enter

As an example, I used the public key from one of my wallets: 0x041fae2190d128f11c79eea67cc28edf514a521c87da553554d529ee7c8ff1e2fcead0da832cf471a91da33d1b3163de5db79f327d1fb1f01ac52d97405e8cfc94

![Image alt](https://github.com/Gene-stack/public-key-to-address/blob/main/img3.jpg)

As you can see in the screenshot, the script successfully calculated the wallet address from the public key.

**For MacOS**

Step 1. Open a terminal

![Image alt](https://github.com/Gene-stack/public-key-to-address/blob/main/img45.jpg)

Step 2. Paste the command and press Enter 

![Image alt](https://github.com/Gene-stack/public-key-to-address/blob/main/img5.jpg)

Step 3. Enter the system password

![Image alt](https://github.com/Gene-stack/public-key-to-address/blob/main/img6.jpg)

Step 4. Input your public key and press Enter

As an example, I used the public key from one of my wallets: 0x041fae2190d128f11c79eea67cc28edf514a521c87da553554d529ee7c8ff1e2fcead0da832cf471a91da33d1b3163de5db79f327d1fb1f01ac52d97405e8cfc94
. You can use the key from my wallet to test the script. The result of the calculation should be the wallet address 0x5b3ed47D33979aABDa952bca8f9C84FC28c3ab2A.
