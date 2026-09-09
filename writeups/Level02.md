# Bandit Level 2 → Level 3

## Objective
Retrieve the password stored in a file named `spaces in this filename` located in the home directory.

## Walkthrough
1. Connect to the OverTheWire SSH server using the `bandit1` account:
    ```bash
    ssh bandit2@bandit.labs.overthewire.org -p 2220
2. List the files in the home directory:
    ```bash
    ls
3. Read the contents of the file
    ```bash
    cat ./"--spaces in this filename--"
where double quotes "" group the spaced arguments into a single filename parameter for cat.
<img width="712" height="92" alt="image" src="https://github.com/user-attachments/assets/f5bfea3f-cdb6-4200-ac07-15ba7b12131e" />
