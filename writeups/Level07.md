# Bandit Level 7 → Level 8

## Objective
Retrieve the password stored in `data.txt` next to the word `millionth`.

## Walkthrough
1. Connect to the OverTheWire SSH server using the `bandit7` account:
    ```bash
    ssh bandit7@bandit.labs.overthewire.org -p 2220

2. List the files in the home directory:
    ```bash
    ls

3. Search `data.txt` for the specific line containing `millionth`:

   ```bash
   grep "millionth" data.txt

<img width="491" height="66" alt="image" src="https://github.com/user-attachments/assets/6144d566-f923-45a2-8cd4-4a9dab64e311" />
