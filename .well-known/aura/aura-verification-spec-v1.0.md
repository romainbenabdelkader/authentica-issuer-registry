# AURA Verification Specification v1.0

Revision: 2026-07-31 (editorial — evidentiary scope wording; no change to
algorithms, canonicalization, hashing or verification steps 1-4)

Issuer: AUTHENTICA-PILOT

Algorithm: Ed25519

Canonicalization: RFC-8785-JCS

Asset hash: SHA3-256

Manifest hash: SHA3-256

Public verification key:

https://issuer.lockdna.tech/.well-known/aura/public-key.pem

Issuer metadata:

https://issuer.lockdna.tech/.well-known/aura/issuer.json

AURA standard DOI (the open standard this specification implements):

10.5281/zenodo.21251473

DOI of this verification specification:

10.5281/zenodo.21723153

Verification steps:

1. Fetch the public key.
2. Canonicalize the manifest without the signature block using RFC-8785-JCS.
3. Verify the Ed25519 signature.
4. For evidence with file integrity, recompute the asset SHA3-256 hash and compare it with the manifest asset hash.
5. For `catalog_claim` evidence, treat file integrity as not applicable: the evidence verifies a signed catalogue declaration with an issuer-declared issuance time, not file content.

AURA verifies integrity, declared metadata and signature validity. The issuance time is issuer-declared unless independent timestamp evidence is provided. It does not prove authorship, ownership, entitlement, grounding, citation or usage completeness.
