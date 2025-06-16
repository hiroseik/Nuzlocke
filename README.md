# Nuzlocke Tracker Prototype

This repository contains a small prototype for tracking Pokémon game progress. It
loads route data from a Google Sheet and displays a dropdown for each route
using React.

## Using Google Sheets as a Data Source

1. Create a Google Sheet with a tab named `Routes`.
2. Add two columns: `Route` and `Pokemon`. The `Pokemon` column can contain a
   semicolon-separated list of Pokémon available on that route.
3. Make the sheet public or publish it to the web so it can be fetched
   anonymously.
4. The sheet can be read as JSON via
   `https://opensheet.elk.sh/<SHEET_ID>/Routes`. Replace `<SHEET_ID>` with your
   sheet's ID. This prototype uses the public sheet with ID
   `16sAyuGi_9KV6Ag64vItbsz7i5jw7xgDNK3bYvHLVNaE` as an example.

## Running the Prototype

1. Open `index.html` in a browser.
2. By default it loads data from the example sheet above. To use your own
   sheet, replace the `sheetId` constant in the inline script with your sheet's
   ID.
3. When the page loads, it fetches the JSON data and renders a dropdown menu for
   each route.

This setup provides a minimal foundation that can be expanded into a richer
application as more features (such as item tracking or statistics) are added.


## Styling the Prototype

The page includes the [Bootswatch](https://bootswatch.com/) "Cosmo" theme. A
copy of the CSS (`cosmo.min.css`) is bundled locally so the page still has the
theme when offline. To try a different theme, download another Bootswatch CSS
file and update the `<link>` in `index.html` accordingly (for example replace
`cosmo.min.css` with `darkly.min.css`).
=======

