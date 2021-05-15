# Working with files

The main function of a text editor is to edit files of text. This means that
one of the most important aspects is to learn how to work with these files.

## Open files 

The first step is to learn how to open files. They can be opened from the
command line by tiping the name of the file after vim like `vim file.txt`
or they can be opened within vim with the command `:e file.txt`.

The file that's currently open in vim is called the **buffer**.

Additionally if you want to copy the contents of one file into the
current buffer, it can be done with the command `:r[ead]`. 
This command can be used in many different combinations.

## Closing a file

Closing files is also important. 
The default should be `:wq` which saves the file 
and closes it or `:x` which saves only when something 
has changed. 
An equivalent to this last is `ZZ` which is nice and fast.

## Saving files

For saving, the command is just `:w` which comes from write. If you add
filename after it changes to that name or saves there if the buffer
had no previous name.

`:sav file.txt` saves to a new file.

## Navigation

Once we know how to open close and save, the next is to know
how to move around. The basic moving around is through the keys `hjkl`
which move the cursor around. The other way is by words this is the 
best and most efficient way and you should get used to it.
This commands come in lowercase and uppercase. The first separates at
any non letter caracter... the latter only by whitespaces. 
They all can take a number as a prefix. 

It's also possible to scroll through pages, to go to specific places 
around the current file and also around the current window.

## Basic search

There are many ways to search, it's always in normal mode.
The main is by typing `/` This will start the search pattern and when you 
press enter, it searches the next occurrence. with `n` you move to the next
and with `N` to the previous.

Excercise: command for finding first match.

**Mine:** `gg/pattern`
**book:** `/pattern ggn`

`?` changes the direction.


Another option is to search for the word currently under the cursor with
`*` forward or `#` backwards.

Another option is to search for the word currently under the cursor with
`*` forward or `#` backwards.
Another option is to search for the word currently under the cursor with
`*` forward or `#` backwards.


## File manager

To move around files and browse, vim comes with netrw. it shows the files
There are many options to it.
