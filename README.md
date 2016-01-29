youstillhavetwoproblems.py
==

Converts regular expressions from Python to Java or Javascript.

Usage:
```
>>> import youstillhavetwoproblems
>>> youstillhavetwoproblems.to_java('{I got 99 problems}')
'\\{I got 99 problems\\}'
```

This module works by translating the output of the internal sre_parse module.
The output of to_python is not guaranteed to match the input: for example,
characters that are allowed to be escaped may be escaped even if they
were not escaped in the input string.

It is guaranteed, though, that every valid regular expression will be
translated into an equivalent regex valid for the target language.

Disclaimer: Some more obscure constructions have not been tested
and may or may not have been implemented yet.

You might still have two problems, but at least one of them
won't be translating regular expressions from Python to Java.

