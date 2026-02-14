
# Disko-1 Disk Image Extraction

This guide provides instructions on how to extract the disk image and find the hidden flag for the **picoCTF Disko-1** challenge.

## Instructions

### 1. Extract the Disk Image
The provided file is a compressed gzip archive. Use the following command to decompress it:

```bash
gzip -d disko-1.dd.gz
```

### 2. Search for the Flag
Once the disk image (`disko-1.dd`) is extracted, you can search for the flag by extracting readable strings and filtering for the "pico" keyword:

```bash
strings disko-1.dd | grep pico
```

## Tools Used
* **gzip**: For decompressing the `.gz` file.
* **strings**: To find printable characters within the binary disk image.
* **grep**: To filter the output and locate the flag. 
