# green

##
Function: colorize logfile output  
inspired/plucks from [@jaw0](https://github.com/jaw0/)'s http://www.tcp4me.com/code/red

## Typical use:
ignore all lines except containing case-insensitve "Important" or "Bad"  
greenize lines containing "important"  
redize lines containg "bad"
```
$ tail -f logfile | green -x -i -green Important -red Bad
```

greenize lines containing "something"  
blueize lines containing "else"  
ignore lines containing "junk"  
display all other lines non-colorized.
```
$ tail -f logfile | green -green something -blue else -blue foo -v junk
```


options specified first have higher priority
