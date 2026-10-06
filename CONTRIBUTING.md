# Contributing

## Contributor License Agreement

Before a first pull request can be merged, you sign the Structured World Contributor License Agreement once, at <https://sw.foundation/cla>. It covers every repository of the organisation and takes a minute: sign in with GitHub, confirm your e-mail address, sign. The `CLA` status on your pull request then turns green by itself.

You keep the copyright in your contribution. If you contribute as part of your job, your employer may also need to sign the corporate agreement; the page above explains when.

## Pull requests

- Open an issue first for anything beyond a small fix, so the approach can be agreed before the work.
- Use a [conventional commit](https://www.conventionalcommits.org/) title for the pull request; it becomes the commit on `main`. A change that breaks the wire or JSON contract carries `!` in the title.
- Run `buf lint`, `buf format --diff --exit-code` and `buf breaking --against '.git#branch=origin/main'` before pushing; CI runs the same checks.
- New fields and messages carry a comment that says what they mean.

## Reporting security issues

Do not open a public issue; see [SECURITY.md](SECURITY.md).
