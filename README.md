# Secret-Santa-Finder
Private Secret Santa helper. Everyone picks who they're buying for and sends back a scrambled link, and the organiser's app works out their own person by elimination. Runs entirely in the browser, with no server, accounts or tracking.

# Secret Santa

Forgot who you drew? This app lets you work it out without anyone finding out who anyone else has.

1. The organiser enters everyone's names and gets a link to share.
2. Each person opens it, picks who they're buying for, and gets a scrambled reply link.
3. The organiser pastes in the replies. Once everyone else's are in, the app shows the one person nobody else picked.

Everything runs in the browser from a single `index.html`. There's no backend, no accounts and no tracking. The organiser's game is saved in localStorage only, and replies are encrypted with AES-GCM using a key that only appears in the shared link.

**Note:** the organiser's own browser holds the key, so the app can't stop a technical organiser from decoding individual replies with developer tools. It just never shows them.

Hosted on GitHub Pages: open the live site, create a game, and share the link.
