

# Curry-Howard Isomorphism in JavaScript

## 1) A&B -> A v B

`A && B === A || B`

## 2) (A& (B V C)) -> ((A& B ) V (A& C))

`(A && (B || C)) === ((A && B) || (A && C))`

## 3) (A -> C) & (B -> C) & Av B -> C

`(A => C) && (B => C) && (A || B) === C`

## 4) (BVC -> A) -> (B -> A) & (C -> A)

`(B || C => A) => ((B => A) && (C => A))`

## 5) (A -> B ) -> (!B -> !A)

`(A => B) => (!B => !A)`

## 6) ((A -> B ) -> C) -> (A -> (B -> C))

`((A => B) => C) => (A => (B => C))`

## 7) (A -> B ) & (A ->!B) -> !A

`(A => B) && (A => !B) === !A`

## 8) Analogs of de Morgan's rules for implication expressible in the intuitionistic calculus of statements

`(A => B) => !(!A || B)`

`(A => B) => (!A && !B)`

## 9) Bottom

`false`