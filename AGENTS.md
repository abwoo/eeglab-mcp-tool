# Repository instructions

## Execution

Use the existing cloud checkout. Run MATLAB and EEGLAB validation in GitHub Actions.
Keep the MCP server and scientific analysis in MATLAB. Do not introduce Python
implementations, interpreter environments, or desktop installation requirements.

## Commit attribution

Before creating a maintainer commit, configure and verify the repository identity:

```sh
git config --local user.name abwoo
git config --local user.email 47317208+abwoo@users.noreply.github.com
git var GIT_AUTHOR_IDENT
git var GIT_COMMITTER_IDENT
```

Do not inherit an unchecked identity from the execution environment. Preserve
existing Claude attribution. The permitted contributor identities are abwoo
and Claude.

When squash-merging, provide an explicit commit message instead of importing
co-author trailers from GitHub's generated message. Include a co-author trailer
only for an actual contribution by abwoo or Claude.
