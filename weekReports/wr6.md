---
Name: Jose Paz
Semester: Spring 2023
Course: CIS 106
---

# Week Report 6

## Wildcards

### * Wildcard

The * wildcard can represent any character, or any number of characters.   It matches anything and nothing.

- Examples:
  - List all of the PDF files in this directory
    - `ls *.pdf`
  - List all of the files and folders that start with the word "Phone"
    - `ls phone*`
  - Delete multiple files that have a certain pattern in their names
    - `rm test*.log`

### ? Wildcard

The ? wildcard can represent any type of character, but can only represent one single character.

- Examples:
  - List all of the PDF files in this directory that only have one character
    - `ls ?.pdf`
  - List all of the files and folders that start with the word "phone" and a single character after it
    - `ls phone?`
  - Delete multiple files that have 2 characters in their name
    - `rm ??.log`

### [] Wildcard

The [] wildcard matches a single character in a range

- Examples:
  - List all files that have a vowel after the letter f
    - `ls f[aeiou]*`
  - List all of the files whose name has at least one number
    - `ls *[0-9]*`
  - List all files that do not have a vowel after the letter f
    - ls f[!aeiou]*

## Brace Expansions

Brace expansion is a feature of bash that allows you to generate arbitrary strings to use with commands.

Examples:
- This will create the three directories in the current directory.
  - `mkdir folder{1,2,3}`
- This will copy three files to the specified diretory.
  - `cp file{1,2,3}.txt /home/jdpaz/Downloads/`
- This will rename the three files in the current directory.
  - `mv testFile{1,2,3}.txt newFile{1,2,3}.txt`

