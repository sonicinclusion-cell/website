# Sonic Inclusion — Signal Cultures

Website for **Signal Cultures**, a series of experimental sound events in Berlin by Sonic Inclusion. Sponsored by Musikfonds / BKM.

Plain HTML, CSS and vanilla JavaScript — no build step, no dependencies.

## Structure

```
index.html      # the whole site: markup, styles, script
images/         # event posters, artist portraits, logos
.nojekyll       # serve files as-is on GitHub Pages
```

## Editing content

All events, artists and image paths live in two objects at the top of the `<script>` in `index.html`:

- `VOLUMES` — one entry per night (date, venue, text, lineup, ticket link, poster)
- `ARTISTS` — one entry per artist (name, optional role); portraits are `images/<id>.webp`

## Contact form

The form validates and shows a confirmation, but sends nothing until you set `ENDPOINT` in the script (e.g. a Formspree URL).

## Hosting

Served by GitHub Pages from the `main` branch, root folder.
