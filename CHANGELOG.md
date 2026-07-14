# Changelog

Since we follow [Conventional
Commits](https://decisions.seedcase-project.org/why-conventional-commits/),
we're able to automatically create formal "releases" of the website based on our
commit messages. Releases in the context of websites are simply snapshots in
time of the website content. We use
[Cocogitto](https://decisions.seedcase-project.org/why-semantic-release-with-cocogitto/)
to be able to automatically create these releases, which uses
[SemVar](https://semverdoc.org) as the version numbering scheme, and
[git-cliff](https://decisions.seedcase-project.org/why-changelog-with-git-cliff/)
to generate the changelog based on the commit messages.

Because releases are created based on commit messages, a new release is created
quite often---sometimes several times in a day. This also means that any
individual release will not have many changes within it. Below is a list of the
releases we've made so far, along with what was changed within each release.

Commits from bots, like `dependabot` or `pre-commit-ci`, are not included in the
changelog.

## [0.1.0] - 2026-07-13

### ✨ Features

- Add Welcome page
  [#6](https://github.com/seedcase-project/data-pkg-guide/pull/6) by
  [`@lwjohnst86`](https://github.com/lwjohnst86)
  ([9955635](https://github.com/seedcase-project/data-pkg-guide/commit/9955635404a44b447678b4805ee5997029fa0665))

### 💄 Styling

- Reformat Markdown by [`@lwjohnst86`](https://github.com/lwjohnst86)
  ([c15e2bf](https://github.com/seedcase-project/data-pkg-guide/commit/c15e2bf5483e91db6db739b1bf2c618dfb0efcb1))
- Rearrange some items on sidebar
  [#10](https://github.com/seedcase-project/data-pkg-guide/pull/10) by
  [`@lwjohnst86`](https://github.com/lwjohnst86)
  ([5fa2c86](https://github.com/seedcase-project/data-pkg-guide/commit/5fa2c8657c1ba22dc1521c82827b4498635054ec))

### 👷 CI/CD

- Add workflows, including website building by
  [`@lwjohnst86`](https://github.com/lwjohnst86)
  ([0e40bd8](https://github.com/seedcase-project/data-pkg-guide/commit/0e40bd80559712f116e36dd45e98dccac89f098d))
- Add missing path to `cog.toml` in `release.yml` workflow by
  [`@lwjohnst86`](https://github.com/lwjohnst86)
  ([c22df5f](https://github.com/seedcase-project/data-pkg-guide/commit/c22df5f1fd92f98a9762f3d49eeeb82364753ee9))
- Fix arg to pass `--config` correctly in `cog check` workflow by
  [`@lwjohnst86`](https://github.com/lwjohnst86)
  ([5813fab](https://github.com/seedcase-project/data-pkg-guide/commit/5813fabbcb3f15f2a7a43ac6640c2dcf301c890a))
- Ignore merge commits with `cog check` by
  [`@lwjohnst86`](https://github.com/lwjohnst86)
  ([04a2e11](https://github.com/seedcase-project/data-pkg-guide/commit/04a2e1142fdf7673f0799ec52f63633154f60269))

### 👩‍💻 Miscellaneous

- Setup repo from template by [`@lwjohnst86`](https://github.com/lwjohnst86)
  ([d5375df](https://github.com/seedcase-project/data-pkg-guide/commit/d5375df56cc3a325764f3da45ccaf286f780f89f))
- Remove `TODO` items by [`@lwjohnst86`](https://github.com/lwjohnst86)
  ([b499267](https://github.com/seedcase-project/data-pkg-guide/commit/b499267520f6e7732e6322a256a4a9b0d5987ae7))
- Add (empty) pages on the sidebar by
  [`@lwjohnst86`](https://github.com/lwjohnst86)
  ([0debc06](https://github.com/seedcase-project/data-pkg-guide/commit/0debc06976b44ee2078308fd38bb3fe4bfbc3f5a))
- Build to PDF via typst by [`@lwjohnst86`](https://github.com/lwjohnst86)
  ([cf549af](https://github.com/seedcase-project/data-pkg-guide/commit/cf549af9ce270bc660e9abaa1e478a770d4b620e))
- Fix issues that arose when building to PDF via typst by
  [`@lwjohnst86`](https://github.com/lwjohnst86)
  ([4e0d123](https://github.com/seedcase-project/data-pkg-guide/commit/4e0d1238b1c53eb04e303e2ca1a7900857d78bbf))
- Add contributor file to fix build issues by
  [`@lwjohnst86`](https://github.com/lwjohnst86)
  ([1d05247](https://github.com/seedcase-project/data-pkg-guide/commit/1d05247ad817d0928e2d5de3d918feda0e6d9f5c))
- Add empty pages to set up structure by
  [`@lwjohnst86`](https://github.com/lwjohnst86)
  ([51fc7d2](https://github.com/seedcase-project/data-pkg-guide/commit/51fc7d2a3da52d51ac1e60f1aef452893c863da9))
- Don't track Quarto-generated `_files/` by
  [`@lwjohnst86`](https://github.com/lwjohnst86)
  ([d6d1aba](https://github.com/seedcase-project/data-pkg-guide/commit/d6d1aba89a2d94b4d63e96da2e8163576237a7b8))
- Don't check `pre-commit.ci` URLs by
  [`@lwjohnst86`](https://github.com/lwjohnst86)
  ([35c8145](https://github.com/seedcase-project/data-pkg-guide/commit/35c814526ba76d57e0ac6d3381fc134ea40fe313))
- Add `#sec-` links to empty pages by
  [`@lwjohnst86`](https://github.com/lwjohnst86)
  ([5210e25](https://github.com/seedcase-project/data-pkg-guide/commit/5210e25312cd9e02985f6a2b1dbf40738f0bb2b2))
- Update the tagline to be more descriptive by
  [`@lwjohnst86`](https://github.com/lwjohnst86)
  ([4bfacce](https://github.com/seedcase-project/data-pkg-guide/commit/4bfacce1b406b2f55ef0e7cb743551f4482b1e9d))
- Move Tools section down in `_quarto.yml` by
  [`@lwjohnst86`](https://github.com/lwjohnst86)
  ([37e62de](https://github.com/seedcase-project/data-pkg-guide/commit/37e62de88a27fbd03bb082d14b82f824904ec76f))
- Don't check for merge commits during release by
  [`@lwjohnst86`](https://github.com/lwjohnst86)
  ([5b60184](https://github.com/seedcase-project/data-pkg-guide/commit/5b6018479d9341081f53412bca942ba7b3442268))
- Add back `{{version}}` tag that Jinja stripped by
  [`@lwjohnst86`](https://github.com/lwjohnst86)
  ([ecb937a](https://github.com/seedcase-project/data-pkg-guide/commit/ecb937affaf96c90900bb5f5d23ab4452711ab55))
- Remove merge commit, so don't need this setting by
  [`@lwjohnst86`](https://github.com/lwjohnst86)
  ([f1d6963](https://github.com/seedcase-project/data-pkg-guide/commit/f1d6963677da7f26a79020f25254bba8e557996a))
- Remove spaces in `{{}}` in `cog.toml`, not allowed by
  [`@lwjohnst86`](https://github.com/lwjohnst86)
  ([00d3a7b](https://github.com/seedcase-project/data-pkg-guide/commit/00d3a7b81e55d1041d333ed4fd18cf00004955f7))

### ❤️ New contributors

- [`@lwjohnst86`](https://github.com/lwjohnst86) made their first contribution
- `@dependabot[bot]` started making automated contributions
