# Bindery

Design a journal, print it in folding order, and get the templates to sew and
case it by hand.

One self-contained HTML file. No build step, no dependencies, no server, no
account. Everything happens in the visitor's browser — the page layout, the
imposition, reading a calendar file, and generating the printable documents.

## Running it

Open `index.html` in a browser. That is the whole thing.

## Hosting it

Any static host works, because there is nothing to run. Drag the folder onto
Netlify Drop, or push this repository and turn on GitHub Pages.

## What it sends anywhere

Nothing. The only outbound request is to Google Fonts for the typefaces. An
imported calendar is read in the browser and never uploaded, and it is kept out
of the shareable configuration code so passing your setup to someone else never
passes on your calendar.

## Licence

Not yet decided.
