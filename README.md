# Gamma receipts

One file per book date. Each holds the SHA-256 of every artifact frozen that night, and the hash of the previous day's file, so the days form a chain.

To verify a file, run `sha256sum <file>` and look for the hash in `days/<date>.json`. A match means that exact file existed by the time the commit landed.

Hashes only: no levels, prices, tickers or file names. `SIGNAL_SPEC.md` is named because it is the pre-registration.

Commit dates are the timestamp. Days before this repo's first push were loaded together, so they prove nothing earlier than that push. A receipt proves a file existed and was not changed. It says nothing about whether any signal works.
