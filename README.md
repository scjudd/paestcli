Pae.st CLI
==========

This project provides a command-line interface to [pae.st](http://pae.st).

## paest arguments
<table>
    <tr><td>-h/--help</td><td>show this help message and exit</td></tr>
    <tr><td>-u URL</td><td>the four-letter 'id' of a snippet to update. i.e. 'ZnfK'</td></tr>
    <tr><td>-l LEXER</td><td>specify the lexer (for syntax highlighting)</td></tr>
    <tr><td>-e EXPIRE_TIME</td><td>specify the lifespan of the snippet (in seconds)</td></tr>
    <tr><td>-L</td><td>prevent editing this snippet?</td></tr>
    <tr><td>-r</td><td>return the 'raw' url?</td></tr>
    <tr><td>FILE</td><td>specify the file to paest</td></tr>
</table>

## example usage

### submit a new snippet (explicitly specifying the lexer as python):
```bash
paest test.py -l python
```

### update an existing snippet (i.e., [ZnfK](http://pae.st/ZnfK)):
```bash
paest test.py -u ZnfK
```

### piping command output to a new snippet, locking it, and returning the 'raw' url:
```bash
whois github.com | paest -L -r
```
