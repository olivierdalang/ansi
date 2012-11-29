ANSI
====

Various ANSI escape codes, used in moving the cursor in a text console or
rendering coloured text.


Example
-------

Print something in bold yellow on a red background:

    >>> from ansi.colour import fg, bg, reset
    >>> print map(str, [bg.red, fg.yellow, 'Hello world!', reset])
    ...

If you like syntactic sugar, you may also do:

    >>> print bg.red(fg.yellow('Hello world!'))
    ...
