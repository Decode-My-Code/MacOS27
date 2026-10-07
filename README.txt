# Safari Notify Me price-drop demo

This is a GitHub Pages-ready demo for filming Safari's macOS 27 **Notify Me** feature.

## Setup

1. Create a new **public GitHub repository**, e.g. `iphone-price-demo`.
2. Upload `index.html`.
3. In GitHub: **Settings → Pages → Deploy from a branch → main → / (root)**.
4. Open the generated `github.io` URL in Safari.
5. Safari Page Menu → **Notify Me**.
6. Describe the change, e.g.:
   **"Notify me when the price of this iPhone drops."**
7. Set the frequency Safari offers you (Safari's Notify Me is not a 1-minute watcher).

## Create the price change

The hosted page reads the `PRICE` constant in `index.html`.

Initial version:
`const PRICE = 86900;`

Commit/publish that version first and create the Notify Me alert.

Then change ONLY:
`const PRICE = 79900;`

Commit the change to GitHub. GitHub Pages will serve the changed HTML at the same URL.

Important: Safari's Notify Me checks the actual hosted webpage. Changing text with Web Inspector or changing a local browser DOM does not create a server-side webpage update for Safari's monitor to detect.

The page is an Amazon-inspired demo for filming; it is not Amazon's actual website.
