# Bandit Level 3 → Level 4

## Objective
Retrieve the password stored in a hidden file inside the `inhere` directory.

## Walkthrough
1. Connect to the OverTheWire SSH server using the `bandit3` account:
    ```bash
    ssh bandit3@bandit.labs.overthewire.org -p 2220

2. List the files in the home directory:
    ```bash
    ls
    
3. Navigate into the `inhere` directory:
    ```bash
    cd inhere
    
4. List all files, including hidden dotfiles:
    ```bash
    ls -al
    
5. Read the contents of the hidden file:
    ```bash
    cat ...Hiding-From-You

<img width="1110" height="237" alt="image" src="https://github.com/user-attachments/assets/f171238a-7f87-495d-88c2-67ddf2ae0293" />

