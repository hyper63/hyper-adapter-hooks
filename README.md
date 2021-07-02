<h1 align="center">hyper-adapter-hooks</h1>
<p align="center">A Hooks port adapter that uses fetch to send webhook events in the <a href="https://hyper.io/">hyper</a>  service framework</p>
</p>
<p align="center">
  <a href="https://nest.land/package/hyper-adapter-hooks"><img src="https://nest.land/badge.svg" alt="Nest Badge" /></a>
  <a href="https://github.com/hyper63/hyper-adapter-hooks/actions/workflows/test.yml"><img src="https://github.com/hyper63/hyper-adapter-hooks/actions/workflows/test.yml/badge.svg" alt="Test" /></a>
  <a href="https://github.com/hyper63/hyper-adapter-hooks/tags/"><img src="https://img.shields.io/github/tag/hyper63/hyper-adapter-hooks" alt="Current Version" /></a>
</p>

---

## Table of Contents

- [Getting Started](#getting-started)
- [Installation](#installation)
- [Methods](#methods)
- [Contributing](#contributing)
- [License](#license)

## Getting Started

```js
import { default as hooks } from "https://x.nest.land/hyper-adapter-hooks@1.0.5/mod.js";

export default {
  app: opine,
  adapter: [
    {
      port: "hooks",
      plugins: [hooks(["DATA:QUERY", "DATA:CREATE_DB"])],
    },
  ],
};
```

## Installation

This is a Deno module available to import from
[nest.land](https://nest.land/package/hyper-adapter-hooks)

deps.js

```js
export { default as hooks } from "https://x.nest.land/hyper-adapter-hooks@1.0.5/mod.js";
```

## Methods

This adapter fully implements the Hooks port and can be used as the
[hyper Hooks service](https://docs.hyper.io/hooks-api) adapter

See the full port [here](https://nest.land/package/hyper-port-hooks)

## Contributing

Contributions are welcome! See the hyper
[contribution guide](https://docs.hyper.io/contributing-to-hyper)

## Testing

```
./scripts/test.sh
```

To lint, check formatting, and run unit tests

## License

Apache-2.0
