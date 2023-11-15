# Missing Semester
## The Shell - Textual interface - old school (focus on bash)
Using the shell
* ```missing:-$``` tells you are on the machine ```missing``` and that your current working directory is ```~``` (short for home). The ```$``` tells you that you are not the root user.
* At this point we can type a command. eg. ```date```
* A command with arguments: ```echo hello```. ```echo``` simply prints. The shell parses the command by splitting by whitespace. If an argument with whitespace, use ```' '``` or ```" "``` to wrap around. Or escape the relevant character with ```\```. ```echo "hello world"``` is equivalent to ```echo hello\ world```.
* It's essentially writing a small bit of code.
* If the shell is asked to execute a command that doesn't match one of its programming keywords, it consults an environment variable ```$PATH``` that lists which directories the shell should search for programs when it is given a command.
    * ```echo $PATH```: execute the program ```echo```, then searches through the ```:```-separated list of directories in ```$PATH``` for a file by that name. 
    * When it finds it, it runs it.
    * We can find out which file is executed for a given program name using the ```which``` program.
    * We can bypass ```$PATH``` entirely by giving the path to the file we want to execute.

Navigating in the shell
* A path is delimited list of directories
    * Separated by ```\``` on Windows
        * There is one root for each disk partition (eg. ```C:\```).
    * Separated by ```/``` on Linux and macOS (main focus)
        * Root of the file system, under which all directories and files lie
        * A file starts with ```/``` is called an absolute path.
        * Any other is relative path - relative to the current working directory, which we can see with ```pwd``` command and change with ```cd``` command.
        * In a path, ```.``` refers to the current directory, and ```..``` to its parent directory.
* To see what lives in a given directory, ```ls```
    * Unless a directory is given as its first argument, ```ls``` will print the contents of the current directory.
    * Most commands accept flags and options that start with ```-``` to modify their behavior.
        * Usually, running a program with the ```-h``` or ```--help``` will print some help text that tells you what flags and options are available.
        * eg. ```ls --help``` tells us: ""
## Editors (Vim)
## Data Wrangling
## Command-line Environment
## Version Control (Git)
## Debugging and Profiling
## Metaprogramming
## Security and Cryptography
## Potpourri