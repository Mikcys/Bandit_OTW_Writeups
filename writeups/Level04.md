# Bandit Level 4 → Level 5

## Objective
Find the only human-readable file located inside the `inhere` directory.

## Walkthrough
1. Connect to the OverTheWire SSH server using the `bandit4` account:
    ```bash
    ssh bandit4@bandit.labs.overthewire.org -p 2220

2.Move to the target directory:
    ```bash
    cd inhere

3. Inspect file types for all files in the folder:
    ```bash
    file ./*
where file ./* checks the data type of every file in the directory, identifying which one contains ASCII text

4. Read the ASCII text file identified from the previous step:
    ```bash
    cat ./-file07
where ./-file07 explicitly opens the ASCII file using relative pathing

<img width="997" height="580" alt="image" src="https://github.com/user-attachments/assets/d0c1afbd-eaf3-4296-ab8c-2f81fbc9305b" />
