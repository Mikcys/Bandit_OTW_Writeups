# Bandit Level 1 → Level 2

## Objective
Retrieve the password stored in a file named `-` located in the home directory.

## Credentials
* **Host:** `bandit.labs.overthewire.org`
* **Port:** `2220`
* **Username:** `bandit1`
* **Password:** *(Password obtained from Level 0)*

## Commands Used
* `ssh` - OpenSSH SSH client
* `ls` - List directory contents
* `cat` - Concatenate files and print on standard output

## Walkthrough

1. Connect to the OverTheWire SSH server using the `bandit1` account:
    ```bash
    ssh bandit1@bandit.labs.overthewire.org -p 2220

2. List the files in the current working directory:
    ```bash
    ls
3. A file named "-" will be displayed
3. Read the contents of the file named -:
    ```bash
    cat ./-
where cat displays file contents and ./- specifies the relative path to prevent cat from interpreting - as standard input (stdin)
<img width="480" height="100" alt="image" src="https://github.com/user-attachments/assets/02e2bff7-2541-473e-a72a-5067b705321e" />
