"""
cargo-raze crate build file.

DO NOT EDIT! Replaced on runs of cargo-raze
"""
package(default_visibility = [
  # Public for visibility by "@raze__crate__version//" targets.
  #
  # Prefer access through "//kythe/rust/cargo", which limits external
  # visibility to explicit Cargo.toml dependencies.
  "//visibility:public",
])

licenses([
  "notice", # ISC from expression "ISC"
])

load(
    "@io_bazel_rules_rust//rust:rust.bzl",
    "rust_library",
    "rust_binary",
    "rust_test",
)


# Unsupported target "rdrand" with type "bench" omitted

rust_library(
    name = "rdrand",
    crate_type = "lib",
    deps = [
        "@raze__rand_core__0_3_1//:rand_core",
    ],
    srcs = glob(["**/*.rs"]),
    crate_root = "src/lib.rs",
    edition = "2015",
    rustc_flags = [
        "--cap-lints=allow",
    ],
    version = "0.4.0",
    tags = ["cargo-raze"],
    crate_features = [
        "default",
        "std",
    ],
)

# Unsupported target "rdseed" with type "bench" omitted
# Unsupported target "std" with type "bench" omitted
