# Bandit Level 14 → Level 15

## Objective
Submit the current level password to port 30000 on `localhost` to retrieve the next password.

## Walkthrough
1. Connect to the OverTheWire SSH server using the `bandit15` account:
    ```bash
    ssh bandit15@bandit.labs.overthewire.org -p 2220

2. Connect to port 30001 using SSL:

This time, don't use nc alone, because nc creates a normal TCP connection.

Use:
    ```bash
    openssl s_client -connect localhost:30001

You'll see a lot of SSL/TLS information. That's normal.

At the bottom, you should get a place where you can enter data.

Paste the bandit15 password and press Enter.

The server should respond with the bandit16 password.
<img width="745" height="60" alt="image" src="https://github.com/user-attachments/assets/a8d04021-4558-4d4c-9e45-cc4307c96730" />

<img width="1191" height="832" alt="image" src="https://github.com/user-attachments/assets/131178ac-3492-4d56-a6be-882868aa3109" />


