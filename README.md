# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

# AIM:
To execute Windows basic commands and batch scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Windows environment installed on the system or installed inside a virtual environment like virtual box/vmware 

### Step 2:

Write the Windows commands / batch file
Save each script in a file with a .bat extension.
Ensure you have the necessary permissions to perform the operations.
Adapt paths as needed based on your system configuration.
### Step 3:

Execute the necessary commands/batch file for the desired output. 




# WINDOWS COMMANDS:
## Exercise 1: Basic Directory and File Operations
Create a directory named "MyLab" on the desktop.


## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\MyLab
```
![image](https://github.com/Anandanaruvi/Windows-basic-commands-batchscript/assets/120443233/28481d9e-b931-4e7a-9529-05ddc6ad013b)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
```
cd %userprofile%\Desktop\MyLab
```
![image](https://github.com/Anandanaruvi/Windows-basic-commands-batchscript/assets/120443233/c202fbd6-2326-4fe5-82e4-c01a9ef3a4df)

```
type nul > MyFile.txt
```
![image](https://github.com/Anandanaruvi/Windows-basic-commands-batchscript/assets/120443233/52e063eb-76ce-47e4-b17d-68b15b38ebd2)

List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
```
dir %userprofile%\Desktop\MyLab

```
![image](https://github.com/Anandanaruvi/Windows-basic-commands-batchscript/assets/120443233/bc8917e5-7adf-4fe0-b876-3e343e0ca3e8)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.****
Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Backup
```
![image](https://github.com/Anandanaruvi/Windows-basic-commands-batchscript/assets/120443233/261c5f28-1c4f-484c-9292-58a5a84ffac5)

```
copy MyFile.txt %userprofile%\Desktop\Backup
```
![image](https://github.com/Anandanaruvi/Windows-basic-commands-batchscript/assets/120443233/c748cf82-73a0-4bd6-b1fa-233d6fbe43e1)

Move the "MyLab" directory to the "Documents" folder.

### COMMAND AND OUTPUT:
```
mkdir %userprofile%\Desktop\Documents
move MyLab Documents
```

![image](https://github.com/Anandanaruvi/Windows-basic-commands-batchscript/assets/120443233/57f648c9-77a9-481c-b423-9ed0bcdb7442)

## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.
### COMMAND:

```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!

```
![image](https://github.com/Anandanaruvi/Windows-basic-commands-batchscript/assets/120443233/6079de6b-59f8-4c79-a650-d432afd4e7f6)

### COMMAND:
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```

### OUTPUT:

![image](https://github.com/Anandanaruvi/Windows-basic-commands-batchscript/assets/120443233/94486fcd-f45c-438a-b2f6-653492f8c748)

### RESULT:

The commands/batch files are executed successfully.
