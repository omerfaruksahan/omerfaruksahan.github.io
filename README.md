# omerfaruksahan.github.io

The developer website for Read Fast.

- `app-ads.txt` lists who may sell the ads in Read Fast (the IAB
  app-ads.txt standard). Ad buyers look for it at the root of the developer
  website named in the app's store listings, which is why it lives here and
  not in the privacy policy's repo. Since Read Fast 1.0.9 the ads come from
  Appodeal, so the file is Appodeal's list, downloaded from the Appodeal
  dashboard (My Account → App-ads.txt). Its AdMob placeholder is replaced by
  our own Google line, and its Meta placeholder is left out, as we have no
  Meta account. Re-download it when Appodeal updates the list.
- `index.html` is the homepage.
- `classics/` holds the free classics Read Fast offers under Add a book
  (from 1.0.10). The app reads `classics/catalog.json` and downloads the
  `.epub` and `.jpg` it names, relative to it. Books are listed in the
  order shown, shortest first; `words` is the count the app's own reader
  gets, for the reading time it shows.
  - Every book is public domain in the US (published in 1930 or earlier)
    and in the EU, UK and Turkey (author, translator and illustrator dead
    by 1955).
  - The files are Standard Ebooks' editions (standardebooks.org), whose own
    work is dedicated to the public domain (CC0). They are copied here so
    that the app never loads the volunteers' servers. The changes from
    theirs: the imprint page is out of the reading order (`linear="no"`),
    so a book opens on its story, and Alice, Through the Looking-Glass and
    Just So Stories have no illustrations, which made them 10 to 25 MB.
    The app shows an EPUB's text only, and every caption is kept.
  - `.jpg` is the book's cover, at 240×360, for the list.

The privacy policy has its own repo, `PRIVACY-FastReaders`, served at
<https://omerfaruksahan.github.io/PRIVACY-FastReaders/>.
