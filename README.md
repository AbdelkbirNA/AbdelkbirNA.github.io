# abdelkbirnainiaa.me

GitHub Pages host for the apex domain **abdelkbirnainiaa.me**.

## Status

Two things are incomplete:

1. The repository contains only a `CNAME` file — there is no `index.html`, so
   the site serves nothing.
2. The custom domain is **not actually bound**. The `CNAME` file names
   `abdelkbirnainiaa.me`, but the Pages configuration reports no custom domain,
   and the site is published at <https://abdelkbirna.github.io/>. Set the
   custom domain under **Settings → Pages** for the file to take effect.

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
