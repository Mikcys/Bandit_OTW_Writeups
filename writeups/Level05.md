# Bandit Level 5 → Level 6

## Objective
Find a file inside `inhere` that is human-readable, 1033 bytes in size, and not executable.

## Walkthrough
1. Connect to the OverTheWire SSH server using the `bandit5` account:
    ```bash
    ssh bandit5@bandit.labs.overthewire.org -p 2220

2. List the files in the home directory:
    ```bash
    ls

3. Search for the file using criteria filters as given in the problem:
    ```bash
    find -type f -size 1033c

4. Read the contents of the discovered file:
    ```bash
    cat ./maybehere07/.file2    

<img width="536" height="142" alt="image" src="https://github.com/user-attachments/assets/0b79d9fb-338d-4755-990a-d8785ac35a71" />
