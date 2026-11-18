# Rust CLI & Systems Rules (`CLAUDE.md`)

Instructions for Claude Code when developing high-performance Rust applications and CLI utilities.

---

```markdown
# Rust Development Guidelines

## Tooling & Architecture
- Rust stable edition (2021)
- `clap` with derive macro for CLI argument parsing
- `tokio` for asynchronous execution runtime (when networking is required)
- `anyhow` for application-level error handling, `thiserror` for library crate errors

## Standards
- Ensure zero compiler warnings and run `cargo clippy -- -D warnings` on all changes.
- Avoid unnecessary `.unwrap()` in production paths; propagate errors using the `?` operator.
- Write unit tests in module submodules `#[cfg(test)]` and integration tests under `tests/`.

## Common Commands
- Build debug binary: `cargo build`
- Run test suite: `cargo test`
- Lint code: `cargo clippy`
```
