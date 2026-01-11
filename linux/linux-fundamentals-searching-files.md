# Linux Fundamentals Part 1 – Step 6: Searching for Files

## Objective
Learn how to search for files and directories in Linux using essential commands. Understand how to locate files efficiently and filter results, building skills for system navigation, troubleshooting, and cybersecurity tasks.

## Environment
- TryHackMe interactive Linux terminal  
- Browser-based Linux environment  

## Tools Used
- Linux commands: `find`, `locate`, `grep`  
- Shell operators: `|`, `>`  

## Steps Performed
1. Opened the TryHackMe Linux terminal in-browser.  
2. Practiced searching for files using the `find` command:  
   - Example: `find / -name "filename"` – searches the entire filesystem for a file named "filename".  
3. Explored searching by file type:  
   - `find /path -type d` – locate directories  
   - `find /path -type f` – locate files  
4. Used the `locate` command to quickly find files in the database:  
   - `locate filename` – returns paths for all files matching the name.  
5. Learned to search within files using `grep`:  
   - Example: `grep "text" filename` – finds lines containing "text" in a file.  
6. Combined commands with **pipes (`|`)** to filter results:  
   - `find / -type f | grep "keyword"` – find files containing a keyword in their path.  
7. Redirected search output to a file for documentation:  
   - `find / -name "*.txt" > output.txt` – saves results in `output.txt`.  
8. Completed all embedded TryHackMe tasks for searching and filtering files.

## Key Commands
```bash
find /path -name "filename"      # Search for files by name
find /path -type d               # Search for directories
find /path -type f               # Search for files
locate filename                  # Quickly find files using database
grep "text" filename             # Search inside files for specific text
|                                # Pipe output between commands
>                                # Redirect output to a file
