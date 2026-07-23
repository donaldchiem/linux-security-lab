# Linux Wildcards

Wildcards allow you to match multiple files without typing every filename.

## Asterisk (*)

Matches zero or more characters.

Examples:

```bash
ls *.txt
ls a*
ls apple.*
```

If no files match the pattern, ls reports an error because the shell leaves the pattern unchanged.

## Question Mark (?)

Matches exactly one character.

Examples:

```bash
ls ?.txt
ls ??.txt
ls a?.txt
```

## Summary

- `*` = zero or more characters
- `?` = exactly one character

The shell expands wildcards before executing the command.
