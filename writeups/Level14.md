# Bandit Level 14 → Level 15

## Objective
Retrieve the password for Level 13 stored in `data.txt`, which is a hexdump of a repeatedly compressed file.

## Walkthrough
1. Use the key and run:
    ```bash
    ssh -i .\sshkey.private bandit14@bandit.labs.overthewire.org -p 2220

2. Then:
    ```bash
    cat /etc/bandit_pass/bandit14

    <img width="542" height="38" alt="image" src="https://github.com/user-attachments/assets/13e9ec6a-4435-4a82-847e-fd1b4a7c888e" />

3.  Send the password to port 30000:
    ```bash
    nc localhost 30000

You should then see the connection waiting for input.

Paste the bandit14 password and press Enter.

If everything is correct, the server will return the password for bandit15.

<img width="542" height="90" alt="image" src="https://github.com/user-attachments/assets/7d52be53-96b2-4d0f-be50-84b6ffe24e54" />


