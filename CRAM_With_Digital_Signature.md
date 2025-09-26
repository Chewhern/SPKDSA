# Challenge–Response Authentication with Digital Signatures

## Registration
1. The client generates a digital signature key pair and keeps the **private key** securely on the device.  
2. The client submits the **public key** to the server, along with an identifier (e.g., Email, Phone Number, Username, or User ID).  

## Login
1. The client requests a **challenge** from the server. The challenge must be generated using a **CSPRNG (Cryptographically Secure Pseudo-Random Number Generator)** or a **TRNG (True Random Number Generator)**.  
2. The minimum challenge length is **128 bits**.  
3. The client receives the challenge.  
4. The client signs the challenge with their **private key**.  
5. The client sends the signed challenge back to the server.  
6. The server verifies the signature using the client’s **public key**.  

---

✅ **Security Benefit:**  
Since the server never stores or handles private keys, the risk of password leakage is eliminated. Even if the server is compromised, attackers cannot steal private keys. This reduces liability for the organization and increases safety for users.  
