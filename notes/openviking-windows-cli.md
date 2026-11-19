# OpenViking: discovering the Windows development CLI

**Project:** OpenViking · **Area:** Windows developer experience · **Outcome:** merged upstream

[PR #7251](https://github.com/volcengine/OpenViking/pull/7251) · [Issue #7249](https://github.com/volcengine/OpenViking/issues/7249)

## Problem

The Python launcher could miss a development executable present as `target/release/ov.exe` on Windows and report that the CLI was unavailable.

## Change

Select the platform-specific executable name during the existing development lookup, while keeping the established development, bundled and PATH lookup order.

## Evidence and scope

The PR reports a focused Windows comparison: the original implementation passed two of three test bodies, while the change passed all three. A Windows subprocess check also exercised the development, bundled and PATH locations. These were bounded checks, not a normal full-package pytest run or a real Rust CLI build; see the PR for the detailed validation and its limits.
