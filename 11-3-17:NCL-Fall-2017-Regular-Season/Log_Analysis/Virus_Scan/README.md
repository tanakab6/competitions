# Virus Scan
A hacker has accidentally leaked a log file from a virus scan that they ran. Analyze it see what you can learn.

## Questions
1. What operating system was this scan run on? (be as specific as possible)
2. How many physical drives are attached to this computer and accessible during the scan?
3. How much total virtual RAM (in MB) does the system have?
4. What company manufactured the computer?
5. How many named user accounts are on the system?
6. What type of filesystem is the operating system installed on?

## Answers
1. Windows 7 Home Premium
2. 2
3. 8192
4. Dell
5. 2
6. NTFS

## Walkthroughs

We can see the OS by looking at line 4 of the file.

We can see the amount of physical drives by viewing lines 187-190 and seeing the accessible drives.

We can see the total virtual RAM in line 182.

We can guess that this is a Dell computer due to Dell drivers being used in lines 7-48.

We can guess the amount of Users by searching for all unique \\Users\\ and counting them up.

We know that this is using NTFS due to line 241.
