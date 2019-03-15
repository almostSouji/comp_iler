# Comp_iler

Sandboxed code execution discord bot.

## Usage

### Code Blocks

````
>```lang
code
```

>options```lang
code
```
````

### Inline Code

```
>`lang code`

>options`lang code`
```

### Examples

````
>```cpp
#include <iostream>

int main()
{
    std::cout << "Hello World!" << std::endl;
}
```

>harmony```js
class Foo {
    bar = 1;
}

console.log(new Foo().bar);
```

>`py print('hello world')`

>e`hs (+) <$> Just 1 <*> Just 2`
````

## Supported Languages and Options

One of the following language codes is set in `lang`.  
Options are optionally set in `options`, which is a semicolon-delimited list of `flag` or `flag=value`. 

- `c` C (GCC 8.2.0)
- `cpp` C++ (G++ 8.2.0)
- `cs` C# (Mono 5.18.0)
    - `e` evaluates a single expression instead of a module
- `fs` F# (FSharp 4.5)
- `go` Go (Go 1.12)
- `hs` Haskell (GHC 8.6.3)
    - `e` evaluates a single expression instead of a module
- `js` JavaScript (Node 11.11.0)
    - `harmony` enables harmony features (`--harmony` on node)
    - `e` prints the result of evaluating the code
- `pas` Pascal (FPC 3.0.4)
- `py` Python (CPython 3.7.2, CPython 2.7.16)
    - `2` runs Python 2 instead of Python 3
