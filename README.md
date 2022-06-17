# Scratch Cryptography Library
Modern cryptography primitives implemented in Scratch, via [Boiga](https://github.com/DavidBuchanan314/boiga)

**IMPORTANT NOTE:** This is a toy. Don't trust these implementations. Although I have implemented constant-time algorithms, there are no guarantees that they're constant time in the Scratch runtime. Furhermore, I think there are some edge-cases in modular multiplication in poly1305 and x25519 that I need to address, which may be security-relevant.

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

Note: Requires Python 3.10

This should produce a sb3 file at `demo/out/Scratch Cryptography Library: Demo.sb3`,
which you can load into Scratch.

The generated scratch code is massive (~4000 blocks), and looks something like this, when artfully aranged:

![image](https://user-images.githubusercontent.com/13520633/174197302-59255d92-577d-4316-a0ff-1f7f32021ba3.png)
