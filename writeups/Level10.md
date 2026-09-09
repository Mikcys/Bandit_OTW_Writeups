# Bandit Level 10 → Level 11

## Objective
Decode the Base64 encoded string stored in `data.txt`.

## Walkthrough
1. Connect to the OverTheWire SSH server using the `bandit10` account:
    ```bash
    ssh bandit10@bandit.labs.overthewire.org -p 2220

2. List the files in the home directory:
    ```bash
    ls

3. Decode the file content:
   ```bash
   base64 -d data.txt

<img width="637" height="108" alt="image" src="https://github.com/user-attachments/assets/20d40c7e-d757-4767-8357-714b76466a48" />
