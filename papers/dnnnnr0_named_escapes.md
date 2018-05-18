# Named character escapes

Document Number: DnnnnR0  
Date: 2018-05-18  
Audience: Evolution Working Group  
Reply-to: cpp@rmf.io

## Motivation

Currently C++ provides four ways to specify characters in string literals:

 1. the character itself in the appropriate source encoding;
 2. the character as a sequence of `\x` escapes that corresponding to the underlying code units of the character;
 3. the character as a `\u` escape that corresponds to the ISO 10646 name of the character;
 4. the character as a `\U` escape that corresponds to the ISO 10646 name of the character;

These last two are the best way to represent specific Unicode characters that may be hard to type, hard to read, or that
cannot be represented in the source encoding. For example, if one wants a string literal with a combining acute accent,
typing `"\u0301"` is easier than producing a combining acute without a base character, and it is guaranteed that it
won't render wonky in a text editor (e.g. the acute could be rendered on top of the opening double quotes, making it
ugly, and above all, easy to miss).

However, `"\u0301"` is hard to read as well: yes, it's unambiguously clear that this is the character U+0301, but in
general there is no way to know what character that is without first looking it up on some table. This solves the
problem of clarity that is inherent with typing the character directly, but in turn it obfuscates the actual character
behind a series of meaningless numbers.

Other programming languages, in particular Python3 and Perl, have solved this obfuscation problem by providing an
alternative character escape mechanism. In these languages, one can specify a character by using its Unicode Name, as
in the following Python3 example:

    >>> print('A\N{COMBINING ACUTE ACCENT}')
    Á

Having this ability enables one to choose between the brevity of "0301" and the clarity of "combining acute accent" as
desired.

This paper proposes the addition of character escape sequences similar to these to C++ string literals.

## Names



## Aliases



## Named Sequences



## Technical Specifications


