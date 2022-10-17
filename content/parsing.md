# Parsing


## Abstract syntax tree

[Abstract syntax tree | Wikipedia](https://en.wikipedia.org/wiki/Abstract_syntax_tree)


## Concrete Syntax Trees

- Tree-sitter https://github.com/tree-sitter/tree-sitter
    * > Tree-sitter is a parser generator tool and an incremental parsing library. It can build a concrete syntax tree for a source file and efficiently update the syntax tree as the source file is edited.
    > -- https://tree-sitter.github.io/tree-sitter/

    * Used by Helix https://github.com/helix-editor/helix


## Parser combinator

[Parser combinator | Wikipedia](https://en.wikipedia.org/wiki/Parser_combinator)

Implementations:
- [Parsec | Wikipedia](https://en.wikipedia.org/wiki/Parsec_(parser))
    * [@Microsoft/**ts-parsec**](https://github.com/microsoft/ts-parsec) in TypeScript.
    * [@jparsec/**jparsec**](https://github.com/jparsec/jparsec) in Java.

- Masala Parser https://github.com/masala/masala-parser
    * "Javascript Generalized Parser Combinators"
    *
    > Masala Parser is inspired by the paper titled: [Direct Style Monadic Parser Combinators For The Real World](https://www.microsoft.com/en-us/research/wp-content/uploads/2016/02/parsec-paper-letter.pdf). \
    > Masala Parser is a Javascript implementation of the Haskell Parsec. It is plain Javascript that works in the browser, is tested with more than 450 unit tests, covering 100% of code lines.

---

FIN.
