# Bandit Level 6 → Level 7

## Objective
Find a file on the server owned by user `bandit7`, group `bandit6`, and 33 bytes in size.

## Walkthrough
1. Connect to the OverTheWire SSH server using the `bandit6` account:
    ```bash
    ssh bandit6@bandit.labs.overthewire.org -p 2220

2. Search the root filesystem for matching file attributes while redirecting permission errors:
   ```bash
   find / -user bandit7 -group bandit6 -size 33c
where / searches the entire filesystem, -user and -group match ownership, -size 33c specifies 33 bytes
<img width="647" height="22" alt="image" src="https://github.com/user-attachments/assets/99153293-e753-4c8b-86b8-3740af2ff8a9" />

3. Read the flag from the returned path:
    ```bash
    cat /var/lib/dpkg/info/bandit7.password
<img width="567" height="35" alt="image" src="https://github.com/user-attachments/assets/380b3650-2a0d-4178-8192-4b37da11f5a8" />




