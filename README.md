<div align="center">
  <h1>lint-staged-commit-all-repro</h1>
  <strong>Project to showcase a bug noticed when using lint-staged with lerna</strong>
</div>

<hr>

# Explanation

The problem arises when you try to commit a change by amending a commit rather than creating a new commit. This works:

- `git add .`
- `git commit --amend --no-edit`

But this does not:

- `git commit -a --amend --no-edit`
