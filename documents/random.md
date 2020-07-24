# random - generate a random number

## Synopsis
```fish
    random
    random SEED
    random START END
    random START STEP END
    random choice [ITEMS...]
```

## Description
`random` generates a pseudo-random integer from a uniform distribution. 
- The range (inclusive) is dependent on the arguments passed. 
- No arguments indicate a range of [0; 32767]
- If one argument is specified, the internal engine will be seeded with the argument for future invocations of `random` and no output will be produced.
- Two arguments indicate a range of [**START**; **END**].
- Three arguments indicate a range of [**START**; **END**] with a spacing of **STEP** between possible outputs.
- `random choice` will select one random item from succeeding arguments.
<br />
- Note that seeding the engine will NOT give the same result across different systems.
- You should not consider `random` cryptographically secure, or even statistically accurate.


## Example

The following code will count down from a random even number between 10 and 20 to 1.

```fish
for i in (seq (random 10 2 20) -1 1)
	echo $i
end
```
___

Open a random .jpg file from any of the subdirectories:
```fish
    open (random choice **jpg)
```

## Source
https://fishshell.com/docs/current/cmds/random.html
