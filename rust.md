# Rust
A checklist for people using Rust to develop Firefox services, to be used in addition to the [common checklist](README.md).

* [ ] Use https://github.com/RustSec/cargo-audit to check for dependency security vulnerabilities
* [ ] Use https://github.com/rust-lang/rust-clippy for linting (easier for new projects)
* [ ] Use https://github.com/mozilla-services/slog-mozlog-json for service logging
* [ ] Binaries (as opposed to libraries) should include a Cargo.lock file in version control
* [ ] Use https://dependabot.com/rust/ to keep your dependencies up to date
* [ ] Only use 'unsafe' when it is absolutely necessary
* [ ] Only use Rust nightly when it is absolutely necessary
  * [ ] If you have to use nightly track the features you require so that you can move of fit once they are merged into stable
* [ ] Minimise dependencies, and only use well regarded and supported ones (not Rust specific, but important due to the relative immaturity of the ecosystem)

## Recommended crates

| Crate | Description |
| ----- | ----------- |
| [Actix](https://crates.io/crates/actix) | Actix is a Rust actors framework. |
| [Hyper](https://crates.io/crates/hyper) | A fast and correct HTTP implementation for Rust. |
| [Reqwest](https://crates.io/crates/reqwest) | An ergonomic, batteries-included HTTP Client for Rust. |
| [Serde](https://crates.io/crates/serde) | Serde is a framework for serializing and deserializing Rust data structures efficiently and generically. |
| [Slog](https://crates.io/crates/slog) | The logging for Rust |

Additional recommendations can be proposed via PRs or issues.

## Markdown issue template
For the above checklist.

```
* [ ] Use https://github.com/RustSec/cargo-audit to check for dependency security vulnerabilities
* [ ] Use https://github.com/rust-lang/rust-clippy for linting (easier for new projects)
* [ ] Use https://github.com/mozilla-services/slog-mozlog-json for service logging
* [ ] Binaries (as opposed to libraries) should include a Cargo.lock file in version control
* [ ] Use https://dependabot.com/rust/ to keep your dependencies up to date
* [ ] Only use 'unsafe' when it is absolutely necessary
* [ ] Only use Rust nightly when it is absolutely necessary
  * [ ] If you have to use nightly track the features you require so that you can move of fit once they are merged into stable
* [ ] Minimise dependencies, and only use well regarded and supported ones (not Rust specific, but important due to the relative immaturity of the ecosystem)
```