### Apply cargo fmt to all rust project from a root directory

`find . -name "*Cargo.toml" -exec cargo fmt --all --manifest-path {} \;`
