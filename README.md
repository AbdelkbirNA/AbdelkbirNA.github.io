# abdelkbirnainiaa.me

GitHub Pages host for the apex domain **abdelkbirnainiaa.me**.

## Status

The custom domain **is** bound — the site is published at
<http://abdelkbirnainiaa.me/>. What is missing is content: the repository holds
only a `CNAME` file, with no `index.html`, so the domain resolves to nothing.

HTTPS is also not enforced yet. Once GitHub has issued the certificate, turn on
**Enforce HTTPS** under Settings → Pages.

## What lives here

| File | Purpose |
|---|---|
| `CNAME` | Binds `abdelkbirnainiaa.me` to this Pages site |

## Publishing a site

Add an `index.html` (or any static build output) to the default branch and
GitHub Pages will serve it at the custom domain. Keep `CNAME` in place — Pages
rewrites or drops the domain binding if that file disappears from the published
branch.

For a framework build, either commit the built output to the branch Pages
serves, or add a workflow that builds and deploys to Pages on push.

## DNS

The apex domain needs `A` records pointing at GitHub's Pages IPs, and
`www` a `CNAME` to `abdelkbirna.github.io`. Enforce HTTPS in the repository's
Pages settings once the certificate is issued.
