...
---

- Shell is command line interpreter.

      Examples shell => Bash, cmd, PowerShell

lets you control the system.

      You → Shell → Operating System

- Bash is the default shell on many systems.

- Terminal is text input/output environment

---

Directories And Files
```
cd [path]                           //move forward
cd ../[path]                        //move back
mkdir [path]
mv [path]      and      mv [old name] [new mane]
cp [path]
touch [files]
rm -d           //remove empty directory and files
rm -r           //force remove directory and files
```
> [!NOTE]
> `\Redirection >` is for saving, sends output to a file.

Cat And Echo
```
echo 'text' > [path file]            //create a file and put text in it
echo 'text' >> [file]           //add text without replacement
cat [files] > [file]            //copying content ⚠️​(use >> to non-replacement)
cat -n [file]                   //show numbers of lines
```
Grep
```
grep 'search text' [file]
grep 'search text' -r [directory]            //search in recursive directories
                   -l                        //Sorting files containing 'search text'
examples:
grep 'error' [file] > [errors file]
piping the results:
ls -l | grep 'search text'
```
> [!NOTE]
> `\Pipe |` is for processing.
> It sends the output of one command to another command.
> Pipe connects stdout to stdin.
> Example:
>       ls | grep ".c"
>       ls → writes to stdout
>       grep → read from stdin












