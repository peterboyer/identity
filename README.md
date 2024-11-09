# identity

## Installation

```shell
npm install pb.identity
```

## Requirements

- `typescript@>=5.0.0`
- `tsconfig.json > "compilerOptions" > { "strict": true }`

# API

- [`Identity`](#identityt)

### `Identity<T>`


```ts
import type { Identity } from "pb.identity";

const value = Object.assign({ A: true }, { B: true });
//    ^ { A: boolean } & { B: boolean }
type Result = Identity<typeof value>;
//   ^ { A: boolean; B: boolean }
```

