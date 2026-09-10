# Bandit Level 12 → Level 13

## Objective
Retrieve the password for Level 13 stored in `data.txt`, which is a hexdump of a repeatedly compressed file.

## Walkthrough

1. Connect to the OverTheWire SSH server using the `bandit11` account:
    ```bash
    ssh bandit11@bandit.labs.overthewire.org -p 2220

2. Create a workspace in the temporary directory to avoid modifying files in your home folder:
   ```bash
   mktemp -d

3. Change location to the temporary directory:
   
```bash
cd <temp_dir_path>

<img width="542" height="66" alt="image" src="https://github.com/user-attachments/assets/83de8118-d1ac-4803-9c00-98234ba59199" />

4. Copy data.txt to the current directory:

```bash
cp ~/data.txt .
where cp copies the original file.

<img width="707" height="71" alt="image" src="https://github.com/user-attachments/assets/2b8b11fd-23fb-4b65-80dd-a412e3fb06f4" />

5. Reverse the hexdump:

```bash
xxd -r data.txt data
where xxd -r converts the ASCII hexdump back into binary format named data.

6. Identify and decompress the first layer (gzip):

```bash
file data
mv data data.gz
gzip -d data.gz
where file reveals gzip compressed data and gzip -d decompresses data.gz back to data

7. dentify and decompress the second layer (bzip2):

```bash
file data
mv data data.bz2
bzip2 -d data.bz2
where file reveals bzip2 compressed data and bzip2 -d extracts it.

8. Identify and decompress the third layer (gzip):

```bash
file data
mv data data.gz
gzip -d data.gz
where file reveals gzip compressed data and gzip -d decompresses it.

<img width="1462" height="360" alt="image" src="https://github.com/user-attachments/assets/3d7d34e5-9ad5-4717-a1fb-595fcfec458d" />

9. Extract the fourth layer (tar archive):

```bash
file data
mv data data.tar
tar -xf data.tar
file *
where tar -xf extracts the contents of data.tar, producing a new file named data5.bin.

<img width="576" height="41" alt="image" src="https://github.com/user-attachments/assets/37ce3152-990e-4cb5-93de-992518e6142f" />

10. Extract the fifth layer (tar archive):

```bash
mv data5.bin data5.tar
tar -xf data5.tar
file *
where tar -xf extracts data5.bin, producing a new file named data6.bin.

<img width="682" height="112" alt="image" src="https://github.com/user-attachments/assets/2d07986c-c2e4-405a-893a-885491247035" />

11. Identify and decompress the sixth layer (bzip2):

```bash
mv data6.bin data6.bz2
bzip2 -d data6.bz2
file *
where bzip2 -d decompresses data6.bz2, resulting in a file named data6.

<img width="840" height="112" alt="image" src="https://github.com/user-attachments/assets/76416b16-1f34-4836-84a5-a23e833330cb" />

<img width="732" height="116" alt="image" src="https://github.com/user-attachments/assets/20a18203-111a-437c-a9ec-6c40e2afe5ca" />

12. Extract the seventh layer (tar archive):

```bash
mv data6 data6.tar
tar -xf data6.tar
file *
where tar -xf extracts data6.tar, producing a new file named data8.bin.

13. Decompress the eighth layer (gzip) and read the flag:

```bash
mv data8.bin data8.gz
gzip -d data8.gz
file data8
cat data8
where gzip -d produces data8 (identified as ASCII text), and cat data8 prints the final password for Level 13.

<img width="1452" height="288" alt="image" src="https://github.com/user-attachments/assets/0459d1e3-f8f0-45a9-b523-7b9b5bf5ee91" />

