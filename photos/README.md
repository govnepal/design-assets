# photos/

Metadata only (`meta/`) — photo binaries live in object storage, referenced by storage_key + sha256 checksum, served via CDN. CI is the only writer to the bucket: staging prefix → PR review → merge promotes + generates derived sizes (thumbs, webp).
