# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

Developed By: Yuvabharathi.B

Reg No: 212222230181

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

mkdir %userprofile%\Desktop\MyLab

![image](https://github.com/AshwinKumar-Saveetha/Windows-basic-commands-batchscript/assets/155129814/30906be8-14a0-42df-be77-32fd1db31b60)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.
## COMMAND AND OUTPUT

cd %userprofile%\Desktop\MyLab

![image](https://github.com/AshwinKumar-Saveetha/Windows-basic-commands-batchscript/assets/155129814/219b74d7-05db-4607-ba11-27751dc8e214)

![image](https://github.com/AshwinKumar-Saveetha/Windows-basic-commands-batchscript/assets/155129814/231c6c4e-3340-415c-953c-3d929983c9ef)


List the contents of the "MyLab" directory.
## COMMAND AND OUTPUT

dir %userprofile%\Desktop\MyLab

![image](https://github.com/AshwinKumar-Saveetha/Windows-basic-commands-batchscript/assets/155129814/26b5dd3d-0930-4a7b-bbc1-b70d2eab433d)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
## COMMAND AND OUTPUT

mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup


![image](https://github.com/AshwinKumar-Saveetha/Windows-basic-commands-batchscript/assets/155129814/4b522d08-477a-4ac2-bdf8-ce34b5377f8a)

![image](https://github.com/AshwinKumar-Saveetha/Windows-basic-commands-batchscript/assets/155129814/2b3d2723-ef8d-47a6-a7a6-d230fc1e3937)


Move the "MyLab" directory to the "Documents" folder.

## COMMAND AND OUTPUT

mv Myfile.txt %userprofile%\Documents

![image](https://github.com/AshwinKumar-Saveetha/Windows-basic-commands-batchscript/assets/155129814/7a71bbce-a804-472a-96be-308a5862f6ba)


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
Modify the script to delete files with the ".docx" extension from the "Documents" folder after creating the backup.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```

## OUTPUT
![image](https://github.com/AshwinKumar-Saveetha/Windows-basic-commands-batchscript/assets/155129814/3d062ebb-7d20-4c09-95dc-b10861f34223)

# RESULT:
The commands/batch files are executed successfully.

