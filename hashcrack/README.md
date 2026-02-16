

### Step 1: Server Connection

First, connect to the server using `nc` (Netcat) with the following command:

```bash
nc verbal-sleep.picoctf.net 57034

```

### Step 2: Cracking the Hashes

Upon connection, the server will prompt you to crack three hashes sequentially. These are common passwords that can be easily decrypted using **CrackStation**.

* **Tool:** [CrackStation]()

### Step 3: Retrieval

1. Copy the hash provided by the server.
2. Paste it into CrackStation to find the plaintext password.
3. Input the cracked password back into the terminal.
4. Repeat this for all three hashes.

After successfully cracking the third password, the server will provide the flag.

