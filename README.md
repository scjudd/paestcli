Pae.st CLI
==========

This project provides a command-line interface to [pae.st](http://pae.st).

## paest arguments
<table>
    <tr><td>-h/--help</td><td>show this help message and exit</td></tr>
    <tr><td>-f FILE</td><td>specify the file to paest</td></tr>
    <tr><td>-u URL</td><td>the four-letter 'id' of a paest to update. i.e. 'ZnfK'</td></tr>
    <tr><td>-l LEXER</td><td>specify the lexer (for syntax highlighting)</td></tr>
    <tr><td>-e EXPIRE_TIME</td><td>specify the lifespan of the paest (in seconds)</td></tr>
    <tr><td>-L</td><td>prevent editing this paest?</td></tr>
    <tr><td>-r</td><td>return the 'raw' url?</td></tr>
</table>

## example usage

### submit a new paest (explicitly specifying the lexer as python):
```bash
paest -f test.py -l python
```

### update an existing paest (i.e., [ZnfK](http://pae.st/ZnfK)):
```bash
paest -f test.py -u ZnfK
```

### piping command output to a new paest, locking it, and returning the 'raw' url:
```bash
whois github.com | paest -L -r
```
