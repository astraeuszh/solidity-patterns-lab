# Solidity Patterns Lab

Solidity Patterns Lab is a focused showcase for Solidity language features and
security patterns. Each example will be small, isolated, documented, and backed
by tests so the repository is useful for review and learning rather than being a
collection of opaque production code.

## Direction

The first milestone is a security-oriented pattern library covering:

- explicit access control and least-privilege roles;
- checks-effects-interactions and reentrancy-resistant value flows;
- pull payments, pausing, and emergency recovery paths;
- custom errors, events, invariants, and gas-aware data structures;
- adversarial tests for authorization, accounting, and failure behavior.

The project is a technical demonstration. It is not an audited protocol and must
not be used to custody real funds without an independent review and deployment
process.

## Layout

```text
src/       Solidity examples, one pattern per contract where practical
test/      Unit, invariant, and adversarial tests
script/    Reproducible local deployment and demonstration scripts
docs/      Design notes, threat models, and review records
```

## Tooling

This repository uses [Foundry](https://book.getfoundry.sh/) for compilation,
testing, formatting, and local execution.

```bash
forge build
forge test
forge fmt --check
```

Before a pattern is marked complete, document its assumptions, trust boundaries,
known limitations, and test coverage in `docs/`.

## Status

The repository currently contains only the reviewed project skeleton. Contract
examples will be added in a separate implementation pass.

## License

MIT. See [LICENSE](LICENSE).
