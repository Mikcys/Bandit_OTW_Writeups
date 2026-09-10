# Bandit Level 13 → Level 14

## Objective
Log into `bandit14` using the private SSH key stored in `sshkey.private`.

## Walkthrough
1. Connect to the OverTheWire SSH server using the `bandit13` account:
    ```bash
    ssh bandit13@bandit.labs.overthewire.org -p 2220

2. List the files in the current working directory:
    ```bash
    ls

3. Read the contents of the file named sshkey.private:
    ```bash
    cat sshkey.private
The private key will be displayed!!

4. Copy the private key into a Notepad

5. Save the key correctly

In Notepad, you should have something that starts like:

-----BEGIN OPENSSH PRIVATE KEY-----

and ends like:

-----END OPENSSH PRIVATE KEY-----

Do not change anything inside it.

In Notepad:
  
    File → Save As

For the filename, enter:
    
    sshkey.private

For Save as type, choose:
 
    All Files (*.*)

And preferably save it somewhere easy, such as:

Desktop 

⚠️ Make sure Windows doesn't save it as:
    ```bash
    ssh.private.txt

6. Now exit from bandit 16
    ```bash
    exit   

7. Will be continued in the next level


