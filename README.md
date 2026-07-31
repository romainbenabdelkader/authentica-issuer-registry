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
