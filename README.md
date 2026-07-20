# Hom3
Desktop, Mobile, custom OS, and Hardware. Mostly source-viewable. 2,600 line rust os may go open source. Mobile HOM3 deck targeting launch on crowd supply.

**Sovereign, local-first computing.**

HOM3 Technologies builds software, hardware, and an operating system for people who want computing that is local, verifiable, and theirs. Everything runs on your machine. Nothing phones home.

[hom3.org](https://hom3.org)

---

## Principles

- **Local-first.** Full function offline. Airgap-capable by design.
- **No tracking.** No analytics, no cookies, no telemetry. Not reduced — absent.
- **Verifiable.** Every release ships with SHA-256 checksums and Ed25519 signatures. Don't trust — verify.
- **Provenance.** Append-only, Bitcoin-anchored logbook for artifacts and events. Patent pending.
- **Yours.** Your keys, your data, your hardware.

## The line

| Project | What | Status |
|---|---|---|
| **HOM3** | Local-first AI workspace — macOS · Windows · Linux | Shipping — [hom3.org](https://hom3.org) |
| **HOM3 Deck** | Handheld sovereign terminal (RK3588) | Crowd Supply, upcoming — [hom3.org/deck](https://hom3.org/deck) |
| **HOM3os** | Purpose-built OS for HOM3 hardware | released Boot-Init MIT — [OS Github](https://github.com/onePaulKrause/hom3init) |
| **identitytrusts** | Provenance & watermarking primitives — Ed25519 · SHA-256 · DCT/QIM | [identitytrusts.org](https://identitytrusts.org) |
| **LVL5** | Falling blocks in five dimensions. Because we could. | [lvl5.hom3.org](https://lvl5.hom3.org) |

## Verify

Release signing key (Ed25519):

```
[PUBLIC KEY — published with the first anchored commit]
fingerprint: [FPR]
```

Checksums and signatures for every shipped build live in [`/proofs`](./proofs), mirrored at [hom3.org](https://hom3.org).

```sh
shasum -a 256 -c SHA256SUMS      # integrity
./verify.sh <artifact>           # signature + logbook anchor
```

If a hash doesn't match, don't run it. Tell us.

## Roadmap

1. Signing key publication + anchor
2. `/proofs` — checksums and signatures for all shipped builds
3. Provenance whitepaper — self-anchored: its own hash sealed in the logbook it describes
4. HOM3os source release
5. HOM3 Deck hardware documentation
6. Packages: Umbrel · Start9

No dates. Hashes first, promises second.

## Manifesto

[hom3.org/manifesto](https://hom3.org/manifesto)

## License

Per-subtree — see `LICENSE` files. HOM3os licensing will be announced with its source release.

---

*Patent pending.*

.-. 1<3 Paul Krause
