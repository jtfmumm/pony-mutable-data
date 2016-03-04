# pony-mutable-data


## mutable-data/List

Helper methods for the "collections" package mutable List

The primitive mutable-data/Lists has the following methods:

```
    contains[A: (Any #read & Equatable[A])](l: List[A], a: A): Bool 

    drop[A: Any #read](l: List[A], n: USize): List[A]

    every[A: Any #read](l: List[A], f: {(A!): Bool} val): Bool

    exists[A: Any #read](l: List[A], f: {(A!): Bool} val): Bool

    filter[A: Any #read](l: List[A], f: {(A!): Bool} val): List[A]

    flat_map[A: Any #read, B](l: List[A], f: {(A!): List[B]} val): List[B]

    flatten[A](l: List[List[A]]): List[A]

    fold[A: Any #read,B: Any #read](l: List[A], f: {(B!, A!): B^} val, acc: B): B

    map[A: Any #read, B](l: List[A], f: {(A!): B^} val): List[B]

    partition[A: Any #read](l: List[A], f: {(A!): Bool} val): (List[A], List[A])

    take[A: Any #read](l: List[A], n: USize): List[A]

    take_while[A: Any #read](l: List[A], f: {(A!): Bool} val): List[A]

    unit[A](a: A): List[A]
```
