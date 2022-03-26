# Minimal Hello World example on Solana Blockchain

This example is heavily influenced by the official [example-helloworld](https://github.com/solana-labs/example-helloworld), but a lot more minimal, in order to be understood as fast as possible:
- Smart contract is only written in Rust.
- No ensuring that program is deployed.
- No Typescript on the client part.
- No NPM scripts that hide the actual commands away (you really should know them!!).
- No tests.

This project wasn't made as a learning source. A lot of the comments are vague or cringe, as I was only trying to explain how it works only to myself.

# Program (Smart Contract)
Increments the number of greetings on the account.


### Build the program:
```console
$ cargo build-bpf
```

### Deploy the program:
```console
$ solana program deploy /target/deploy/helloworld.so
```

# Javascript Client
Interacts with the on-chain program. Creates accounts if nescessary.

### Start the client:
```console
$ node /client/src/index.js
```