"""
cargo-raze crate build file.

DO NOT EDIT! Replaced on runs of cargo-raze
"""
package(default_visibility = [
  # Public for visibility by "@raze__crate__version//" targets.
  #
  # Prefer access through "//remote/non_cratesio/cargo", which limits external
  # visibility to explicit Cargo.toml dependencies.
  "//visibility:public",
])

licenses([
  "notice", # "MIT"
])

load(
    "@io_bazel_rules_rust//rust:rust.bzl",
    "rust_library",
    "rust_binary",
    "rust_test",
)



rust_library(
    name = "redox_termios",
    crate_root = "src/lib.rs",
    crate_type = "lib",
    srcs = glob(["**/*.rs"]),
    deps = [
        "@non_cratesio__redox_syscall__0_1_37//:redox_syscall",
    ],
    rustc_flags = [
        "--cap-lints=allow",
        "--target=x86_64-unknown-linux-gnu",
    ],
    version = "0.1.1",
    crate_features = [
    ],
)
