# builtin - run a builtin command

## Synopsis
```fish
    builtin [OPTIONS...] BUILTINNAME
    builtin --query BUILTINNAMES...
```

## Description
`builtin` forces the shell to use a builtin command, rather than a function or program.

The following parameters are available:
- `-n` or `--names` -- List the names of all defined builtins
- `-q` or `--query` -- Tests if any of the specified builtins exists

## Example
```fish
    # executes the jobs builtin, even if a function named jobs exists
    builtin jobs
```

## Source
https://fishshell.com/docs/current/cmds/builtin.html
