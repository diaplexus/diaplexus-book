# Programming Languages

## Elm - [http://elm-lang.org](http://elm-lang.org)

_"A delightful language for reliable webapps. Generate JavaScript with great performance and no runtime exceptions."_

Authored by Evan Czaplicki - [http://evan.czaplicki.us/](http://evan.czaplicki.us/)

Elm is a functional language inspired by and written in Haskell. It seems to aim to employ a minimal subset of Haskell's features striking a balance between high utility and ease of access. The language compiles to Javascript and utilizes a port system for typed interop with the Javascript ecosystem.

Some notable features include:

* Union types.
* Embedding as a DOM element.
* Enforced semantic versioning for package ecosystem.
* The Elm Architecture - [https://guide.elm-lang.org/architecture](https://guide.elm-lang.org/architecture)
  * A model-update-view pattern for centralized model state where messages, which are often a union type, are mapped to a specific update of the model.
  * [https://dennisreimann.de/articles/elm-architecture-overview.html](https://dennisreimann.de/articles/elm-architecture-overview.html)
* No runtime errors.
* Efficient virtual DOM.

#### Code Example

Quick Sort - [http://elm-lang.org/examples/quick-sort](http://elm-lang.org/examples/quick-sort)

```elm
import Html exposing (text)


main =
  text (toString (quicksort [5,3,8,1,9,4,7]))


quicksort : List comparable -> List comparable
quicksort list =
  case list of
    [] ->
        []

    pivot :: rest ->
        let
          lower  = List.filter (\n -> n <= pivot) rest
          higher = List.filter (\n -> n >  pivot) rest
        in
          quicksort lower ++ [pivot] ++ quicksort higher
```

## Nim - [https://nim-lang.org/](https://nim-lang.org/)

_"Efficient and expressive programming. Nim is a systems and applications programming language. Statically typed and compiled, it provides unparalleled performance in an elegant package._

_High-performance garbage-collected language_

* _Compiles to C, C++ or JavaScript_
* _Produces dependency-free binaries_
* _Runs on Windows, macOS, Linux, and more"_

## Haskell - [https://www.haskell.org/](https://www.haskell.org/)

_"An advanced, purely functional programming language."_

## Elixir - [https://elixir-lang.org/](https://elixir-lang.org/)

_"Elixir is a dynamic, functional language designed for building scalable and maintainable applications._

_Elixir leverages the Erlang VM, known for running low-latency, distributed and fault-tolerant systems, while also being successfully used in web development and the embedded software domain."_

## Eve - [http://witheve.com/](http://witheve.com/)

_"Eve is a modern relational language for writing data-driven programs without the boilerplate."_

## Unison - [http://unisonweb.org/](http://unisonweb.org/)

_"Next generation programming platform, currently in development."_

_"Unison is a new programming platform that rethinks just about every aspect of the programming experience."_

## Spry - [http://sprylang.org/](http://sprylang.org/)

"Spry borrows homoiconicity from Rebol and Lisp, free form syntax from Forth and Rebol, the word of different types from Rebol, good data structure literal support from JavaScript and the general coding experience and style from Smalltalk. It also has a few ideas of its own, like an interesting argument passing mechanism and a relatively novel take on OO."



