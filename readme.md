# Kismet Crest HOA

A one-page website for the Kismet Crest Homeowners Association on Kismet Way in
Eugene, Oregon. It covers the community layout (the recorded plat map), dues,
the key rules from the CC&Rs, the recorded documents, and how to reach the
board. The page is kept short enough to print on two pages.

The page is plain HTML and CSS. There is nothing to install and no build step.

## Updating the page

Open `index.html` in any text editor and search for `EDIT ME`. Each of those
notes marks a part meant to be changed and never shows up on the page.

| What you want to change         | Search for                                 |
| ------------------------------- | ------------------------------------------ |
| Name, tagline, location         | `EDIT ME: association name`                |
| Dues amount and due date        | `EDIT ME: dues amount`                     |
| Recorded documents              | `EDIT ME: documents`                       |
| Board email                     | `EDIT ME: contact details`                 |
| Title in the browser tab        | `EDIT ME: your page title`                 |
| Colors, fonts, spacing          | the top of `styles.css`                    |
| Logo                            | `assets/logo.svg`                          |
| Plat map image                  | `assets/plat-map.png`                      |

The layout description and the key-rules summary come from the recorded plat
and CC&Rs. If the association amends its CC&Rs, update those sections too.

Change the words between the tags, not the tags themselves. To add another
document, copy one whole block from `<li>` to `</li>`, paste it below, and edit
the copy.

To publish documents, create a `documents` folder next to `index.html`, put the
PDFs in it, and link each document title in the documents section to the
file's path, such as `documents/ccrs.pdf`. Leave out anything private, such as
owner contact lists or financial account details: this page is public.

## What's in here

```
index.html      the page itself: all of the words and links
styles.css      how it looks: colors, fonts, spacing
script.js       the light/dark switch and the copy-link button
assets/         the logo and the plat map
favicon.svg     the small icon in the browser tab
```

## Good to know

- Light and dark both work. The page follows the device setting, and the
  switch in the corner overrides it and remembers the choice.
- It works with a keyboard and with screen readers.
- Printing the page (or saving it as a PDF) gives a two-page handout. The print
  layout hides the toolbar and section links.
- Keep the PDFs small: the whole site should stay under a megabyte. The original
  scanned CC&Rs file is about 6 MB, so compress it or split it before uploading.
