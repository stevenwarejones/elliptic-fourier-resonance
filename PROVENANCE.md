# Provenance

This repository extracts the focused elliptic companion study from
[ramanujan-series PR #3](https://github.com/stevenwarejones/ramanujan-series/pull/3),
source commit
[`1801d9509f5b62401d55ec4af6c6cd02a76b343e`](https://github.com/stevenwarejones/ramanujan-series/commit/1801d9509f5b62401d55ec4af6c6cd02a76b343e).

The source study occupies `research/elliptic-companions/`, with its regression
tests in `tests/test_elliptic_companions.py`. It was introduced in one commit;
that commit is a research checkpoint, not a chronological record of every
exploration. The original commit and PR remain available for review. This
standalone repository records the source explicitly rather than presenting
rewritten extraction commits as the original Git history.

On extraction, the mathematical notes, verifier implementations, and four
certificate snapshots are unchanged. The test import path is adjusted to the
new root. The README, contribution guidance, and CI are adapted to a standalone
repository. No additional mathematical result is claimed by this migration.

The project was developed with AI assistance. Its claims should be assessed
from the derivations, cited literature, and independently replayable checks;
passing tests does not replace mathematical review.
