# Search and Filter utility in Linux-
Search utilities are used to search files from the system where as filter utilities filters the 
output. Following are some filter tools that can we use:

## sort –
- Sorts the lines alphabetically by default but there are many options available to modify the sorting mechanism.
- sort filename
#### options-
- -r: Reverse the sort order
- -n: Sort numerically
- -o: Output the result to a file


## sed – 
- sed stands for stream editor.
- It allows us to apply search and replace operation on our data effectively.
#### options:
* s: substitute occurrence of a pattern with a replacement
- sed 's/old/new/' filename
* p: Print the lines that match a pattern.
- sed -n '/pattern/p' filename
* -i: Edit the file in place (i.e., modify the original file)
- sed -i 's/old/new/' filename
* d: Delete lines that match a pattern
  -sed '/pattern/d' filename.
## wc –
- wc command gives the number of lines, words and characters in the data.
#### Options:
- -l Show Line Count
- -w Display word count
- -m Show character count
## grep – 
- grep is used to search a particular information from a text file.
- grep 'pattern' filename

#### Options:
- -v Invert match.
- -c Output count of matching lines only.
## find –
- Find command is used to search and locate the list of files and directories based on conditions you specify for files that match the arguments.
- Find can be used in a variety of conditions like you can find files by permissions, users, groups, file type, date, size, and other possible criteria.
- Syntax:
#### find <search_path> <options> <required-parameters>
##### Options,
- -name <file_name>
- Search for a file with the specified name
- -perm <mode>- File's permission bits are exactly mode (octal or symbolic)
- -user <name>- File is owned by user specified
- -group <grp_name> - File is owned by group specified.
- -empty- The file is empty
- -executable - The file is executable
- -readable- Find files which are readable
- -writable- Search for files that can be written to
- -type <type>- Search for a particular type (f,d,l,c,b,s,p)





