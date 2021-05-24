# Substitution

This chapter cover substitution technics which comes really handy when editing files. The main idea is that substitution is done in command mode
and follows the following pattern: `:s/bad/good/g`. This command is based on the idea of searching for a word `bad` and replacing for `good`. 
By default, this command is applied in the current line only, so it is very important to first understand ranges:

## Ranges

The range is where in a buffer does the command takes place. By defauld, most commands apply only to the current line `.`.
The range modification should be specified right after the colon in the command and is a line number or the line range to apply the command
using the key `%` it applies to the whole file and so on. 

## Search and replace

The basic command for search and replace goes like the following: `:[range] s[ubstitute]/pattern/string/[flags] [count]` where everything between brackets
is optional. Range defines where to apply the command, the pattern to search and the string is the replacement. The flag defines how to do the operation,
for example `g` changes everything or `c` asks for confirmation before every replacement. Multiple flags can be used. 

Some important patterns to remember is to use `\<` and `\>` in order to match only whole words or use `\|` for logical OR in order
to match one pattern OR the other and replace. 

Without flag, it defaults to replace only the first match in the range. With `g` it replaces every match. With `c` I can use
an interactive display to move through the matches and select which to replace.

## Search through multiple files

The command `:vimgrep` allows you to search for a pattern in multiple files. It is followed by the string and then some patter for the files to search in, for example `*.md`
for markdown files.

For example, a recursive search that includes subdirectories requieres a file pattern of the type `**/*.md`.
