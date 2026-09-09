# Bandit Level 9 → Level 10

## Objective
Find the human-readable string in binary file `data.txt` preceded by several `=` characters.

## Walkthrough
1. Connect to the OverTheWire SSH server using the `bandit9` account:
    ```bash
    ssh bandit9@bandit.labs.overthewire.org -p 2220

2. List the files in the home directory:
    ```bash
    ls

3. Extract readable text and search for string patterns:

   ```bash
   strings data.txt | grep "="

<img width="581" height="277" alt="image" src="https://github.com/user-attachments/assets/08d3f5a4-fe70-4aa0-8ac9-e1adf567eb32" />

