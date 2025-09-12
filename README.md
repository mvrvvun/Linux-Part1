# 🐧 Learn Linux - Level 1 Cheat Sheet

A concise **Linux command cheat sheet** for beginners and intermediate users covering essential terminal operations.

---

## 📑 Table of Contents
1. [User Management & Permissions](#user-management--permissions)
2. [System Update & Upgrade](#system-update--upgrade)
3. [File & Directory Management](#file--directory-management)
4. [Searching & Text Processing](#searching--text-processing)
5. [System Monitoring & Management](#system-monitoring--management)
6. [Experimentation & Customization](#experimentation--customization)

--- 
# 🔹 User Management & Permissions
sudo adduser Marwane      # Create a new user named Marwane
sudo cat /etc/shadow      # Show encrypted passwords (requires root)
sudo cat /etc/passwd      # Show user account info

# 🔹 System Update & Upgrade
sudo apt-get update       # Update package lists from repositories
sudo apt-get upgrade      # Upgrade installed packages to latest versions

# 🔹 File & Directory Management
ls                        # List files and directories
ls -alt                   # List all files with details, sorted by modification time
ls -a                     # List all files including hidden ones
ls -l                     # Long listing: permissions, owner, size, date
pwd                       # Show current working directory
cd ..                     # Move to parent directory
cd /../                    # Move up one level (from root’s parent)
rm filename               # Delete a file
rmdir foldername          # Remove an empty directory
rm -r foldername          # Remove a directory and all its contents recursively
cp source dest            # Copy file or directory (use -r for directories)
mv source dest            # Move or rename file/directory
touch filename            # Create empty file or update its timestamp
cat filename              # Display contents of a file
nano filename             # Open file in nano editor
echo "hello" > file       # Write "hello" to a file (overwrite)
echo "hello" >> file      # Append "hello" to the end of a file

# 🔹 Searching & Text Processing
grep pattern file         # Search for a text pattern in a file
grep -I pattern file      # Search ignoring binary files
grep env file             # Example: search for "env" in a file
wc filename               # Count lines, words, characters in a file
sort filename             # Sort lines alphabetically
uniq filename             # Remove duplicate consecutive lines (use after sort)

# 🔹 System Monitoring & Management
lsof -i -n -p             # List open network files/processes
man command               # Show manual page for a command

# 🔹 Experimentation & Customization
sed 's/amal/Marwan/' Marwane.txt > new.txt  # Replace "amal" with "Marwan" in a file and save to new.txt
nano ~/.bashrc            # Edit the current user's bash configuration
source ~/.bashrc          # Reload bash settings immediately
