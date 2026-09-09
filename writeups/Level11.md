# Bandit Level 11 → Level 12

## Objective
Decode `data.txt`, which has been rotated by 13 positions (ROT13 cipher).

## Walkthrough
1. Connect to the OverTheWire SSH server using the `bandit11` account:
    ```bash
    ssh bandit11@bandit.labs.overthewire.org -p 2220

2. List the files in the home directory:
    ```bash
    ls

3. Apply character translation to shift alphabetic characters:

   ```bash
   cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'

<img width="570" height="68" alt="image" src="https://github.com/user-attachments/assets/94ab1860-dcd3-4cc7-8abb-f352708c01c0" />
