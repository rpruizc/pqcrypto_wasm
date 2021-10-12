# PQCrypto for WASM

The Post-Quantum Standarization competition has
reached its third round (https://csrc.nist.gov/Projects/post-quantum-cryptography/). Few algorithms are left as finalists to be standardized and real-world implementations are emerging. In this project, I want to broaden the field of implementations.

WebAssembly (WASM - https://webassembly.org/) is a portable binary-code format for
executable programs including a textual representation
for programs. 

The main goal of WASM is to enable high-performance applications on web pages, but the format is designed to be executed and integrated in other environments as well, including standalone ones.

>The idea is to take PQCRYPTO algorithm implementations (e.g. Kyber or Saber) and compile them for WASM targets.

>Kyber - https://pq-crystals.org/

>Saber - https://www.esat.kuleuven.be/cosic/pqcrypto/saber/

Besides potential non-optimality of compiler output, security issues such as random number generation need to be considered and evaluated. The second step is thus an evaluation of the status quo of WASM runtimes. 

Depending on my advance, I may shift the focus to optimization (w.r.t. memory or runtime) or recommendations to increase security in the WASM runtime.

## Goals and Tasks
- Compile rust/C/pqm4 implementation to WASM
- Verify correctness in browser setup
- Optimize or evaluate security in WASM