# PoseidonCompat

PoseidonCompat is a compatibility plugin for running legacy Project Poseidon plugins on Poseidon v2. It packages dependencies that were available to older plugins but are not supplied by Poseidon v2.

The initial release includes [JSON Simple](https://github.com/fangyidong/json-simple) 1.1.

## Requirements

- Poseidon v2.0.0 or newer
- Java 25

## Installation

1. Download `PoseidonCompat-<version>.jar` from the GitHub Releases page.
2. Place it in the server's `plugins` directory.
3. Restart the server.

Plugins that require this compatibility layer should declare it in `plugin.yml` so Poseidon loads it first:

```yaml
depend:
  - PoseidonCompat
```