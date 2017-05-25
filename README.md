# awk-toturial

- The basic function of awk is to search files for lines that contain patterns.
    When a line matches one of the patterns, awk performs speciafied actions on that line.
    The awk continues to process input lines until it reaches the end of the input files.
- Awk are data dirven.

- A rule consists of a pattern followed by an action. the action is enclosed in braces to seprate
    it from the pattern.

    ```
    pattern { action }
    pattern { action }
    ...
    ```

## the way to run awk

```
    awk 'program' in put-file1 input-file2 ...

    awk -f program-file input-file1 input-file2 ...
```

- awk executes statements associated with BEGIN before reading any input.

## awk syntax
```
    gawk [ POSIX or GNU style options ] -f program-file [ -- ] file ...

    gawk [ POSIX or GNU style options ] [ -- ] program-text file ...
```

## The awk language

- because most of files don't contain any of the shell's special characters,so don't need
    to single quotes around the filename that you specify with -f.

- in a file like this #!/bin/awk -f

- the null string is character data that has no value.It is written in awk programs like this:"",in bash
    shell it can be written using "" or ''.
    although the null string has no characters in it, it does not exist.

- null strings are removed when the occur as part of a non-null conmmand-line argument,while
    explicit null objects are kept.

    ```
    awk -F "" 'program' files # correct

    awk -F"" 'program' files # wrong
    ```

### the way to run awk

### regular expressions

### read input files

### print output

### expressions

### patterns, actions,and variables

### arrays in awk

### functions


## Problem solving in awk
### lib of awk functions



## Gawk
### Advanced features of gawk

### internationalization with gawk

### debugging awk programs

### arithmetic and arbitrary-precision arithmetic with gawk

### writing extensions for gawk

## example

```
awk 'BEGIN { print "Don\47t Panic!" }'

awk '{ print }'
```

- set +H disable C shell-style command history
