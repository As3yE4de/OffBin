
# README
## Usage
To print usage, simply type the tool's name and hit Enter.

`.\Splitter_v1.0.0.1.exe <FILE> [<COMMAND(S)>]`

**FILE**

This argument is an absolute path to a specific file. If there are spaces in the name of the file, enclose it with the quotation marks.

**COMMANDS**

`--size=<SIZE>`  Specify the size of splitted fragments. This value takes a number (without 
any suffix, it is considered as byte), if --size option is not specified, 512 bytes would be used. 
The suffix can be used including: K (kilobyte), M (megabyte), or G (gigabyte).

`--out=<PATH>`  Specify the destination path for the splitted fragments to be saved.
The destination path must be an absolute path. If --out option is not specified, the current 
directory would be used.

## Examples
To split a file into smaller fragments which have 512 bytes and are saved at the current directory, use the following command:

`.\Splitter.exe C:\Users\User\Test\test.txt`

<img width="686" height="924" alt="image" src="https://github.com/user-attachments/assets/b6765278-10cc-47f1-a999-1cccd911392f" />

To split a file into smaller fragments which have 1024 bytes and are saved at the specified directory, use the following command:

`.\Splitter.exe C:\Users\User\Test\test.txt --size=1024 --out=C:\Users\User\Test\Frags`

or

`.\Splitter.exe C:\Users\User\Test\test.txt --size=1K --out=C:\Users\User\Test\Frags`

<img width="906" height="689" alt="image" src="https://github.com/user-attachments/assets/a93faf92-3a8c-4d9f-a5f4-02c415f01cbf" />

## Tested environment
- Windows 10 x64

---
