# Bandit Level 8 → Level 9

## Objective
Find the only line of text in `data.txt` that occurs only once.

## Walkthrough
1. Connect to the OverTheWire SSH server using the `bandit8` account:
    ```bash
    ssh bandit8@bandit.labs.overthewire.org -p 2220

2. List the files in the home directory:
    ```bash
    ls

3. Sort lines alphabetically and filter out duplicates:
   ```bash
   sort data.txt | uniq -u

<img width="412" height="72" alt="image" src="https://github.com/user-attachments/assets/7909cf36-05d4-4ba4-aca1-a19491b97ce5" />
