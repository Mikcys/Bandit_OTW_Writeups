# Bandit Level 12 → Level 13

## Objective
Retrieve the password for Level 13 stored in `data.txt`, which is a hexdump of a repeatedly compressed file.

## Walkthrough

1. Create a workspace in the temporary directory to avoid modifying files in your home folder:

   ```bash
   mktemp -d
