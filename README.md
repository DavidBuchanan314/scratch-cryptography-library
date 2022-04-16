# Scratch Cryptography Library
Modern cryptography primitives implemented in Scratch, via [Boiga](https://github.com/DavidBuchanan314/boiga)

## Algorithms:

- BLAKE3 (https://github.com/BLAKE3-team/BLAKE3-specs)
- BLAKE2s ([RFC-7693](https://datatracker.ietf.org/doc/html/rfc7693))
- ChaCha20 ([RFC-8439](https://datatracker.ietf.org/doc/html/rfc8439))
- ChaCha20-based CSPRNG
- ChaCha20-Poly1305 ([RFC-8439](https://datatracker.ietf.org/doc/html/rfc8439))
- x25519 ([RFC-7748](https://datatracker.ietf.org/doc/html/rfc7748)) (EC scalar multiplication, suitable for ECDH)

### Getting the source:

```
git clone --recursive https://github.com/DavidBuchanan314/scratch-cryptography-library
```

### Compiling the demo:
```
python3 -m demo
```

This should produce a sb3 file at `demo/out/Scratch Cryptography Library: Demo.sb3`,
which you can load into Scratch.
