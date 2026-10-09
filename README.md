# Armature home page

A single static page: `index.html`, `styles.css`, the logo files in `brand/`, the favicon and the bundled fonts in `fonts/`.
No build step, no server code, no outside requests, so it works on any web host.

## Where it lives

The live site is **https://www.armaturelegal.com**, published free by GitHub Pages from the public repo
`stacysubscribes49-gif/armature-site`. That repo holds a copy of this folder; the app code stays private.
`CNAME` tells GitHub Pages the domain; `.nojekyll` makes it serve the files exactly as they are.

## DNS at GoDaddy (My Products → armaturelegal.com → DNS)

Delete any existing `A` record for `@` (the GoDaddy "Parked" one) and any `CNAME` for `www`, then add:

| Type | Name | Value |
| --- | --- | --- |
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |
| CNAME | www | stacysubscribes49-gif.github.io |

`armaturelegal.com` then forwards to `www.armaturelegal.com`. After the DNS has taken effect (minutes to a few
hours), tick **Enforce HTTPS** in the armature-site repo under Settings → Pages.

To preview locally, open `index.html` in a browser.
