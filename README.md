# block-linker

A minimal blockchain prototype in Java with proof of work mining. The project demonstrates block chaining, hash linking and a simple mining loop as a foundation for future applications.

Each block contains its hash, previous hash, payload and nonce. Mining iterates the nonce until the hash meets the difficulty target.

## Why this exists

The goal is to show the core mechanics of a chain without relying on an external ledger. It is a learning prototype, not a production network.

## Features

- Block structure with SHA-256 hash
- Chain validation by hash and previous hash
- Proof of work mining with adjustable difficulty
- Simple in memory chain

## Project structure

```text
.
├── src
│   └── main/java
└── README.md
```

## Prerequisites

Java 17 or later and Maven or direct javac.

## Usage

```bash
git clone https://github.com/mastaan66/block-linker.git
cd block-linker
javac src/main/java/*.java -d out
java -cp out Main
```

Adjust difficulty in the source to see mining time change.

## Limitations

- No networking, consensus or persistence
- Not secure or performant for real use

## Contributing

Issues and pull requests are welcome.

## License

MIT. See LICENSE.
