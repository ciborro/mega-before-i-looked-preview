# mega-before-i-looked-preview

Public review preview of [rig](https://github.com/ciborro/mega-before-i-looked)'s digest page, served by GitHub Pages at https://ciborro.github.io/mega-before-i-looked-preview/.

No HTML is committed here. The `preview` workflow runs rig, saves `/digest/<night>` with `curl` and deploys it (rig ADR 0003). Run it again with `with_marker=false` to replace the page with one whose banner reads "no marker set".

```sh
gh workflow run preview.yml -f with_marker=true    # publish with the lane marker
gh workflow run preview.yml -f with_marker=false   # upload over the same link without it
```
