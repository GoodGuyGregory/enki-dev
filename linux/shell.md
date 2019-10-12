## Usefull Shell Commands:
----------------------------

### Basic Environment Variables:

* **HOME**, Which contains the current user's home directory
* **PATH**, which contains a list of directory paths. When a user types a command without providing the full path *bash* will look at the directories in the PATH environment variable to see if they contain the given command.
* **PS1**, specifies how the prompt is displayed

* **EDITOR**, which specifies the default text editor.

using the `env` command to see a list of all your variables

### Advanced cd tips

**pushd** 

the pushd command saves the current working directory in memory so it can be returned to at any time.

**popd**

 the popd command returns to the path at the top of the directory stack.

 ```shell
[/usr/ports]$ pushd /etc

/etc /user/ports

[/etc]$ popd

/user/ports

[/usr/ports]$

 ```

 **dirs** 

 to list all directories *remembered* directories use `dirs` command:

 ```shell
[/usr/ports]$ dirs

/usr/ports
```

**dirs -c**

to clear the dirs stack use `dirs -c` if you need to revisit the path befor clearing or popping use the change directory with a `-` as below:

`$ cd -`

this will undo the last change of dir and go back to the last visited path


 ```shell
[/usr/ports]$ dirs -c

[]$ dirs
```

**lynx**

it is possible to browse websites from the terminal using the lynx package

 ```shell
$ linyx https://google.com
```

to install use `lynx-cur` package on debian systems

`$ sudo apt-get install lynx-cur`