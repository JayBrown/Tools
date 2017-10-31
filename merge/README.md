![Tools-platform-macos](https://img.shields.io/badge/platform-macOS-lightgrey.svg)
![Tools-code-shell](https://img.shields.io/badge/code-shell-yellow.svg)
[![Tools-license](http://img.shields.io/badge/license-MIT+-blue.svg)](https://github.com/JayBrown/Tools/blob/master/license.md)

# Command Line Tools: merge <img src="https://github.com/JayBrown/Tools/blob/master/img/jb-img.png" height="20px"/>
```
merge v1.0.1

merge <dir 1> ... <dir n> <file 1> ... <file n>
	Merges directory contents or files into "Merged Folder" and retains the directory structures

merge deduplicate <dir 1> ... <dir n> <file 1> ... <file n>
	Retains directory structures, but deletes all duplicate files
	Note: one file per duplicate list is moved to the "_saved" directory
	Note: deduplication is based on checksums, not filenames

merge flatten <dir 1> ... <dir n> <file 1> ... <file n>
	Moves all files to the root of the merge directory and deletes all duplicates
	Note: flatten does not work together with deduplicate

GENERAL NOTES:
	Specifying only one file path will only work if the directory "Merged Folder" already exists
	merge will use the parent directory of the first specified path as its working directory
```
