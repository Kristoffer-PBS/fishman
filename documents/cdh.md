# cdh - change to a recently visited directory

## Synopsis
```fish
    cdh [ directory ]
```

## Description
`cdh` with no arguments presents a list of recently visited directories in the current interactive shell instance.
You can then select one of the entries by or number.

You can also press __tab__ to use the completion pager to select an item from the list.

Note that the `cd` command limits directory history to the 25 most recently visisted directories. 
The history is stored in the `$dirprev` and `$dirnext` variables which this command manipulates.

If you make those universal variables your `cd` history is shared among all fish instances. 

## See Also
See also the `prevd` and `pushd` commands which work with the recent `cd` history and are provided
for compatibility with other shells.

## Source
https://fishshell.com/docs/current/cmds/cdh.html#cmd-cdh
