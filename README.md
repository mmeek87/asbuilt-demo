# AsBuilt demo: Fern & Field

A tiny fictional shop that shows [AsBuilt](https://mmeek87.github.io/AsBuilt/) at work. Every pull request gets its own preview, and AsBuilt checks that preview against what we said we wanted, then comments on the pull request with Pass, Fail or Not verified and screenshots.

## Try it

1. Fork this repository and turn on GitHub Pages for the `gh-pages` branch (Settings → Pages).
2. Open a pull request that changes `site/`.
3. Watch the **Preview and AsBuilt** workflow, then read the AsBuilt comment on your pull request.

The checks live in [`.asbuilt/`](.asbuilt/), one file per feature, written in plain language and reviewed like any other change.

## What's here

- `site/`: the shop (plain HTML and CSS)
- `.github/workflows/preview.yml`: publishes each pull request to `https://<owner>.github.io/asbuilt-demo/pr-<number>/` and runs AsBuilt against it
- `.asbuilt/`: the approved checks

Real apps usually get previews from their host, such as Vercel. For those, the workflow is shorter; see the [AsBuilt setup guide](https://github.com/mmeek87/AsBuilt/blob/main/docs/github-action.md).

Everything here is fictional. No payments are taken.

MIT licensed.
