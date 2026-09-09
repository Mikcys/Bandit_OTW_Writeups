# Bandit Level 0 → Level 1

## Objective
Log in to the game using SSH on port 2220.

## Given Credentials
* **Host**: `bandit.labs.overthewire.org`
* **Port number**: `2220`
* **Username:** `bandit0`
* **Password:** `bandit0`

## Walkthrough (type this in powershell)
1. Connect to the OverTheWire SSH server:
   ```bash
   ssh bandit0@bandit.labs.overthewire.org -p 2220
where ssh denotes the protocol and -p means port which is 2220
2. enter password
3.  ```bash
   ls
   where ls means to list the files and directories in your current location
4. A readme file will be displayed
5. ```bash
   cat readme
   where cat is used to display the contents of a file in the terminal
   <img width="996" height="234" alt="image" src="https://github.com/user-attachments/assets/6907ccdc-2b2e-4ea3-8b49-f6b25eb08392" />

