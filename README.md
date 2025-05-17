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
![image](https://github.com/user-attachments/assets/739f77b0-5837-4a2d-bb82-b0e776265d5f)



Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT

```
cd %userprofile%\Desktop\MyLab
```
![image](https://github.com/user-attachments/assets/1e2c6e96-aa42-4a8a-871a-92739e59a4db)



type nul > MyFile.txt
![image](https://github.com/user-attachments/assets/0f0d4856-c9a6-4243-820a-92dff9d6940f)



List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT

```
dir %userprofile%\Desktop\MyLab
```
![image](https://github.com/user-attachments/assets/7e2e5aac-e838-4a78-8cb1-41f1a6429951)


Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT

```
mkdir %userprofile%\Desktop\Backup
```
![image](https://github.com/user-attachments/assets/ceb1a0e9-70e6-40e3-b96e-093f4da94702)


copy MyFile.txt %userprofile%\Desktop\Backup

![image](https://github.com/user-attachments/assets/6941cf48-fe5a-407c-952e-3533f2e6198a)


Move the "MyLab" directory to the "Documents" folder.

## COMMAND AND OUTPUT

```
mkdir %userprofile%\Desktop\Documents
```
move MyLab Documents
![image](https://github.com/user-attachments/assets/c12fa0f1-0460-4cdf-86b4-f4d6c9f3a3ce)


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

## COMMAND

```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```

## OUTPUT
![image](https://github.com/user-attachments/assets/02641980-802d-4da5-8789-476a451d45a4)


## COMMAND
```
  @echo off
  mkdir %userprofile%\Desktop\DocBackup
  copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
  del %userprofile%\Documents\*.docx
  echo Backup and deletion completed successfully!
```
## OUTPUT
![image](https://github.com/user-attachments/assets/e63af5af-dc1e-469a-befd-5194a784d043)


# RESULT:
The commands/batch files are executed successfully.

