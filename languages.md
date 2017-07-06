# Programming Languages

## \[Elm\]\([http://elm-lang.org](http://elm-lang.org%29%29\)

Authored by  \[Evan Czaplicki\]\([http://evan.czaplicki.us/](http://evan.czaplicki.us/%29%29\)

Elm is a functional language inspired by and written in Haskell. It seems to aim to employ a minimal subset of Haskell's features striking a balance between high utility and ease of access. The language compiles to Javascript and utilizes a port system for typed interop with the Javascript ecosystem.

Some notable features include:

* Union types
* Embedding as a DOM element
* Enforced semantic versioning for package ecosystem
* \[The Elm Architecture\]\([https://guide.elm-lang.org/architecture/](https://guide.elm-lang.org/architecture/%29%29\)\)
  * A model-update-view pattern for centralized model state where messages, which are often a union type, are mapped to a specific update of the model.
  * [https://dennisreimann.de/articles/elm-architecture-overview.html](https://dennisreimann.de/articles/elm-architecture-overview.html)
* No runtime errors
* Efficient virtual DOM

#### Code Example

\[Quick Sort\]\([http://elm-lang.org/examples/quick-sort](http://elm-lang.org/examples/quick-sort%29%29\)

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


