# Undo and Redo

You can undo and redo changes easily. Then main method is with `u` for undo and `Ctrl-r` for redo.
Both this commands can be prefixed with a number to undo or redo a certain number of changes.

You can also use the commands `:ea[rlier]` or `:lat[er]` with a number to move to a future or past state
This commands work with a number for the number of chenges or with a time. So if you want to delete the
last hour you write `:ea[rlier] 1h`. 

## Undo branches

If I edit something, undo it and then edit other thing, undo and redo won't take me back to the original edit.
Vim creates undo branches that let me go back to the previous state of undo. Using `g-` and `g+` will move you between
this branches and will allow you to go to every possible text state you have been. 

## Persistent undo

It is possible to make Vim save a history of undo and redo in a hidden file. (Set this file locations in the `.vimrc`)
This makes it possible to go through your undo and redo branches even through different sessions.
