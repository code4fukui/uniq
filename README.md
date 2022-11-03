uniq
====
Removes all duplicates from an array in place.

Usage
=====
First install using npm:

    npm install uniq

```javascript
import uniq from "uniq";
```

Or import for browsers and deno:

```javascript
import uniq from "https://code4fukui.github.io/uniq/uniq.js";
```

Then use it as follows:

```javascript

var arr = [1, 1, 2, 2, 3, 5]

uniq(arr)
console.log(arr)

//Prints:
//
//  1,2,3,5
//
```

**Returns:** A reference to `array`

**Time Complexity:** `O(array.length * log(array.length))` or `O(array.length)` if `sorted`


## Why use this instead of underscore.uniq[ue]?
A few reasons:

* This library updates the array in place without making an extra copy (and so it is faster for large arrays)
* It also accepts a custom comparison function so you can remove duplicates from arrays containing object
* It is more modular in the sense that it doesn't come with a bazillion other utility grab bag functions.

# Credits
(c) 2013 Mikola Lysenko. MIT License
