# AUTHENTICA Issuer Registry

Public issuer metadata for the AUTHENTICA-PILOT AURA issuer.

This repository contains only public verification material:

- `.well-known/aura/issuer.json`
- `.well-known/aura/public-key.pem`
- `.well-known/aura/aura-verification-spec-v1.0.md`

It does not contain private keys, credentials, manifests, PDFs, client catalogues,
batch reports, or internal AUTHENTICA implementation code.

## Active Issuer

- Issuer: `AUTHENTICA-PILOT`
- Algorithm: `Ed25519`
- Active key id: `authentica-pilot-737817cd43fa1f63`
- Public key DOI: `10.5281/zenodo.21270518`
- Verification spec DOI: `10.5281/zenodo.21723153`
- Public verifier: `https://verify.aura-standard.org/web/`

## Version references

`aura-verification-spec-v1.0.md` is the AUTHENTICA-PILOT issuer's own
verification document, archived under DOI `10.5281/zenodo.21723153`.
Its `v1.0` numbering is separate from AURA-STANDARD releases, manifest schema
versions and AURA-VERIFIER releases. Its historical standard reference is
preserved; it does not describe every check added to later verifier versions.

The published reference verifier is
[AURA-VERIFIER v1.2.0](https://github.com/romainbenabdelkader/AURA-VERIFIER/releases/tag/v1.2.0),
archived under [DOI 10.5281/zenodo.23857156](https://doi.org/10.5281/zenodo.23857156).
Its [integrator guide](https://github.com/romainbenabdelkader/AURA-VERIFIER/blob/6b1a631a9febdd724cfa819c67ec9d285179c27c/INTEGRATORS.md)
defines the implemented local key-status checks. AURA-STANDARD's latest
archived release is [v1.2.1](https://doi.org/10.5281/zenodo.22071523), retaining
manifest schemas 1.0 and 1.1. AURA verification does not require this particular
issuer or registry host.

## Revocation

The former key `authentica-pilot-a5bb72ba62a58e2a` is revoked and must not be
trusted. Revocation metadata is published in `.well-known/aura/issuer.json`.

## Scope

AURA evidence establishes signed, independently verifiable technical claims. The
issuance time is issuer-declared unless independent timestamp evidence is
provided. It does not prove authorship, ownership, entitlement, grounding,
citation or usage completeness.

## License

License: Apache-2.0. See `LICENSE`.
