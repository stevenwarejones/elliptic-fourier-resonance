# Contributing

Keep proved statements, numerical observations, and open questions distinct.
State the exact function family and coefficient field for any exclusion claim;
a functional exclusion does not establish independence at a special value.
Cite primary sources, and do not infer novelty from a failed literature search.

Run the standard-library checks from the repository root:

```sh
python -m unittest discover -s tests -v
python verify_fourier.py
python verify_bounded_reduction.py
```

Do not use Python's `-O` flag, which disables assertions. Scripts write to
stdout and should leave the checkout clean. Put exploratory outputs under
ignored `results/latest/`. Update certificate snapshots only with a documented
reason and a review of the associated proof and error bounds.

For geometry or path changes, also install `requirements-audit.txt` and run
`audit_geometry.py` and `check_torus_path.py`. The latter provides floating-point
cross-checks, not certified interval quadrature. The optional audits can also
be triggered manually in GitHub Actions.

Explain mathematical changes in NOTE.md or BOUNDED_REDUCTION.md, including the
scope, branch/path conventions, evidence, and remaining limitations. Keep the
README accessible and focused on what the work establishes. Use fenced math
blocks and explicit braces for superscripts for GitHub rendering.
