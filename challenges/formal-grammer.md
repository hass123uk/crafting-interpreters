```
expression     → literal
               | unary
               | binary
               | grouping ;

literal        → NUMBER | STRING | "true" | "false" | "nil" ;
grouping       → "(" expression ")" ;
unary          → ( "-" | "!" ) expression ;
binary         → expression operator expression ;
operator       → "==" | "!=" | "<" | "<=" | ">" | ">="
               | "+"  | "-"  | "*" | "/" ;
```

Challenge: Generate a few expressions using this grammar. Can you make it generate anything wrong like 1 + / 3?

I could not.

```
expression -> literal -> "true"

expression -> binary -> 1 + "true"

```
