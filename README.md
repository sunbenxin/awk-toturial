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



