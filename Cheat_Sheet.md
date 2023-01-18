# Terminal & Git Cheat Sheet 

## Terminal Commands

The terminal allows you to access both visible and hidden files without the need of a GUI (Graphic User Interface).

The way which you communicate with the terminal is determinted by what OS (operating system) the computer is running on. Linux and Mac's both operate on a UNIX based OS. The terminal on Mac's allow for the language 'Bash' to be used to communicate with the OS.

***Terminal Navigation***

- `~` **: Tilde** - home directory.
- `pwd` - present working directory.
- `cd` - Home directory.
- `cd /path` - change directory. use `TAB` to autocomplete directory and file names.
- `cd ..` - return to parent directory.
- `cd -` - Return to last location. usefull when visiting deeply nested files and accidentaly returning to home directory for example.
- `ls` - list all visible files with the exception of hidden files.
- `ls -a` - Lists all files including hidden files.
- `ls -l` - Displays more details including permissions, levels, contents, dates ect.
- `ls - al` - list all files, including hidden files in detail.


***Directory & File Naming Conventions***
 
 It is crucial to follow the appropriate namning convetions to avoid errors. It is heavily not recommended to use "space" in file names.The two most popular convetions are:
 
 - snake_case

    snake case are words connected with an "_". Files and Documents following this convetion are usually lowercase for easier termninal navigation.

 - CamelCase
    
    Camel Case uses both Higher and lower case letters to seperate words.

***Creation & Deletion***

- `mkdir` directory_name - create a new directory/folder.
- `touch` new_file.extension - create a new file dependant on the extension such as txt, js, html, css, md.
- `open` - "directory_name/file_name"
- `open .` -  "directory_name"

The following commands delete the file without the file/folder without the option for recoverability. This cannot be reversed. 

- `rm` new_file.txt - delete a file.
- `rm -r` directory_name - delete a directory.

The "r" is recursive. This will delete directories.

***Changing Names & Location***

- `mv` my_file.txt my_other_file.txt - renames file.

- `mv` my_file.txt parent_directory.txt - moves file to different destination.

***General Terminal Commands***

- `TAB` - auto complete for faster navigation.

- `History` -Displays the last 10,000 commands in the terminal.

- `Up/Down arrow keys` - Scroll through the last 5 commands in the terminal.

- `Clear / Ctrl L` - create blank space within terminal for easier readability in the terminal.

- `Command +/-`
Increase/Decrease text size within terminal.

- `Command + T` - Open new tab within terminal.

## Git Commands

Git is a version control system.

Github is the most popular tool for sorting and sharing remote repos.

1. `git init` - initialises a new Git repository within the current directory.

2. Create a new SSH repo on Github.com and copy the line that ends with the following instruction: git@github.com:redacted/random_project.git. Paste it in the terminal.

3. `git add . / git add new_file.md` - Add All files within this directory OR selected the file.

4. `git commit -m'Git Initialized'` - commit staged changes with appropriate and clear message.

5. `git push origin main` - push changes from local host to Github.

***General Git Commands***

`rm -r git` - removes git repository.

`git log` - Displays commit history for the currently active branch.

`git status` - displays wether current changes are 'staged' or 'unstaged'.
- Green - staged.
- Red - Unstaged.

`.gitignore` - create a file with this name to add files you do not want git to track. This will make sure the files are ommited once you git `push origin main`. To add a file, simply type it <filename.extension>

`git rm --cached <file.txt>` - if you are already tracking an unwanted file, this will remove it from the repo however you will still have it locally.