# The Bindery

https://thebindery.org

Design a book, print it in folding order, and get the templates to sew and
case it by hand.

`index.html` is the entire site. No build step, no dependencies, no server,
no database, no account. The page layout, the imposition, reading a calendar
file, and generating every printable document all happen in the visitor's
browser. Nothing is uploaded.

## Deploying

Any static host works, because there is nothing to run.

- **Build command:** none
- **Publish directory:** the repository root
- **Node version:** not required

On Kinsta Static Site Hosting, connect this repository and leave the build
command empty. On Netlify or Cloudflare Pages, the same. On GitHub Pages,
enable Pages for the branch.

## Notes for whoever hosts it

The typefaces are embedded in the file, so it makes no request to any other
host, and makes no request of any kind once loaded. That puts the page at about 1.8 MB, which
compresses to roughly 1.3 MB in transit. Make sure the host serves it gzipped
or with brotli; every static host above does by default.

The page carries its own Content Security Policy in a meta tag, including a
hash of its inline script. **If you edit the JavaScript, that hash has to be
recomputed or the browser will refuse to run the page and it will load blank.**

## Licence

Not yet decided. The embedded typefaces are all under the SIL Open Font
License: Archivo, Fraunces, Outfit, Atkinson Hyperlegible, Libre Caslon Text,
Libre Franklin, Bitter, Cabin, and IBM Plex Mono.
