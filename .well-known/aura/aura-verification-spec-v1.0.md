# AURA Verification Specification v1.0

Issuer: AUTHENTICA-PILOT

Algorithm: Ed25519

Canonicalization: RFC-8785-JCS

Asset hash: SHA3-256

Manifest hash: SHA3-256

Public verification key:

https://issuer.lockdna.tech/.well-known/aura/public-key.pem

Issuer metadata:

https://issuer.lockdna.tech/.well-known/aura/issuer.json

Zenodo DOI:

10.5281/zenodo.21251473

Verification steps:

1. Fetch the public key.
2. Canonicalize the manifest without the signature block using RFC-8785-JCS.
3. Verify the Ed25519 signature.
4. For evidence with file integrity, recompute the asset SHA3-256 hash and compare it with the manifest asset hash.
5. For `catalog_claim` evidence, treat file integrity as not applicable: the evidence verifies a timestamped catalogue declaration, not file content.

AURA establishes technical facts and does not decide legal ownership.
