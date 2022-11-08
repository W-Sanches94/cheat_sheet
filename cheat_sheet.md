# Terminal & Git Cheat Sheet #

## Terminal ##

The terminal allows you to access both visible and hidden files without the need of a GUI (Graphic User Interface).

The way which you communicate with the terminal is determinted by what OS (operating system) the computer is running on. Linux and Mac's both operate on a UNIX based OS. The terminal on Mac's allow for the language 'Bash' to be used to communicate with the OS.

**Terminal Navigation**

insert image
~ home directory

```
pwd
Shows current location and path
```

```
**ls** 
Lists all visible files with the exception of hidden files.
```

```
ls -a
Lists all files including hidden files.
```

```
ls -l
Displays more details including permissions, levels, contents, dates ect.
```

```
ls -al
List all files, including hidden files in detail.
```

```
cd
Change Directory. This followed by directory name will navigate you there. 
Used by itself it will return to the user's home directory.
```

image directory tree illustration.
```
cd .
current directory
```

```
cd ..
parent directory
```

```
cd - 
go back to last location. usefull when visiting deeply nested files and accidentaly returning to home directory for example.
```
**Directory & file creation**
 
 It is crucial to follow the appropriate namning convetions to avoid errors. The two most popular convetions are:
 
 - snake_case

    snake case are words connected with an "_". Files and Documents following this convetion are usually lowercase for easier termninal navigation.

 - CamelCase
    
    Camel Case uses both Higher and lower case letters to seperate words.
```
mkdir "directory_name"
Create a directory / folder.
```

```
```
## Git ##
