# RegExp Summary

*`name`*: uppercase letters

Regexp | Description
--- | --- |
   `a(?=b)` | *matches `a` only if it is followed by `b`*
   `a(?!b)` | *matches `a` only if it is not followed by `b`*
   `(?<=b)a` | *matches `a` only if it is preceded by `b`*
   `(?<!b)a` | *matches `a` only if it is not preceded by `b`*
   `(?:a)` | *matches `a` but does not remember the match*
   `[^abc]` | *matches A `negated or complemented character`set*
   `\d` | *Matches `a digit character`. Equivalent to `[0-9]`*
   `\D` | *Matches `a non-digit character`. Equivalent to `[^0-9]`*
   `\w` | *Matches `any alphanumeric character including the underscore`. Equivalent to `[A-Za-z0-9_]`*
   `\W` | *Matches `any non-word character`. Equivalent to `[^A-Za-z0-9_]`*
   `\b` | *Matches `a word boundary`*
   `\B` | *Matches `a non-word boundary`*
   `\s` | *Matches `white space character, including space, tab, form feed, line feed.`*

   Flag | Description
--- | --- |
   `g` | *Global search*
   `i` | *Case-insensitive  search*
   `m` | *Multi-line search.*
