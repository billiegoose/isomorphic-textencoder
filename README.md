# isomorphic-textencoder
encode/decode Uint8Arrays to strings

To perform UTF8 conversion in the browser it uses the native TextEncoder. In Node it uses native Buffer methods. This is just a thin wrapper that provides an isomorphic API.

## Installation

```sh
npm install isomorphic-textencoder --save
```

## Usage

```js
import { encode, decode } from "isomorphic-textencoder";

encode('Hello') // Uint8Array [ 72, 101, 108, 108, 111 ]

decode(new Uint8Array([72, 101, 108, 108, 111])) // 'Hello'
```

## Dependencies

None

## Dev Dependencies

None

## License

MIT
