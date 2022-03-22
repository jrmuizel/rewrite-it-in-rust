# rewrite-it-in-rust

## Converting from C

### do while loops
There are a couple of different options:
1. `loop { [body] if !condition { break } }`
2. `while { [body] condition } {}`
3. `'outer: loop { loop { [body with continue replaced with break and break replaced with break 'outer ] break; } if !condition { break } `

