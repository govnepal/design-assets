# design-assets

Asset catalog for the depot: emblems, illustrations, photos, animations.

## Storage model (hybrid)
- **In git:** all `meta/` YAML (the catalog), small vector exports (SVG), Lottie JSON,
  emblem masters (high-governance: the audit trail is the point).
- **In object storage + CDN:** photos, videos, high-res exports, editable sources.
  Metadata references them via `storage_key` + sha256 `checksum`. No Git LFS.

CI is the only writer to the bucket: binaries land in a staging prefix, the PR carries
the metadata, and merge promotes the file to the public prefix + generates derived sizes.

Emblem/flag/map masters are restricted-license, status `official` only, and are the
files referenced by the `identity/` specs in design-guidelines.
