# Security Policy

## Reporting a vulnerability

Use this repository's **Security → Report a vulnerability** tab (preferred),
or email **security@kxco.ai**. Do not open public issues for security
reports. PGP key available on request.

We acknowledge reports within **48 hours** and credit reporters in release
notes unless they request otherwise.

## Disclosure

We follow coordinated disclosure with a **90-day** default window. For
actively-exploited issues we ship a patch release within 48 hours.

## Recognition

Valid reports are credited in release notes unless the reporter requests
otherwise. A paid bug-bounty program is under consideration; until one is
announced, rewards are at KXCO's discretion for high-impact findings.

## Scope

In scope: the code in this repository as published to package registries
under the KXCO name.

Out of scope: bugs in the underlying audited primitives — report those
upstream to [`@noble/post-quantum`](https://github.com/paulmillr/noble-post-quantum).

## Our cryptography policy

Every algorithm we ship is NIST-standardized — ML-DSA-65
([FIPS 204](https://csrc.nist.gov/pubs/fips/204/final)) and ML-KEM-768
([FIPS 203](https://csrc.nist.gov/pubs/fips/203/final)) — built on
independently audited implementations. We do not write custom cryptographic
primitives. An independent audit of our own wrapper code is on our roadmap;
until it completes, we state plainly: the primitives are audited (Cure53,
2024), our layer above them is not yet.
