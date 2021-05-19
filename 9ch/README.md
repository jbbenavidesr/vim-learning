# Do you speak Vim?

Vim works like a language and once you learn some basic verbs, nouns and words you can do many things.

## Vim language elemenets

Vim elements can be classified in 3 categories: Verbs, modifiers and nouns.

### Verbs

Usually known as operators, this are the commands that do a certain action. 
Some are powerless because they act in only one character like `x`, `X`, `s` or `r`.

Others are powerfull because they can act in lots of characters, words, paragraphs, etc.
These are for example: `y`, `c`, `d` or `v` (The last one is not really a verb but can act as one.

### Modifiers

These are used before nouns to modify them, for example changing number or specifying a context.

### Nouns

Also known as motions, these describe that to which the action is performed like `w` for words or `p` for paragraph
among many others. Conbined with the appropriate modifier thay can be very powerful like `iw` is inner word to change
the whole word no matter where in it am I standing or `it` for changing content in an HTML tag.

## Learn to talk to Vim

The structure of the sentences is <verb><modifier><noun> and you can use them to form sentences of different actions.

## The dot command

All actions that change something can be repeated easily with the `.` dot command. It repeats the last command which
modified something and can be used with number of repetitions for example. It doesn't repeat motions.
