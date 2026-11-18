# Nueve reinas y NN: vocabulario y lecturas

A class study site for two Latin American films:

- **Nueve reinas** (Fabián Bielinsky, Argentina, 2000)
- **NN: Sin identidad** (Héctor Gálvez, Perú, 2014)

The site has:

- Vocabulary for each film with Spanish meanings and English glosses, plus a practice mode that hides the answers
- Reviews and readings in Spanish and English, marked by difficulty
- Ideas for connecting the two films

The whole site is one file, `index.html`, with no build step. Open it in a browser to view it locally.

## Updating the content

Vocabulary and readings come from the class Google Sheet, which is published to the web as CSV. The site downloads it on every visit, so edits to the sheet show up on the site within about 5 minutes (Google caches the published copy for that long). No commit is needed.

- **vocabulario** tab: `pelicula`, `palabra`, `significado`, `english`, `ejemplo`, `categoria`
- **resenas** tab: `pelicula`, `titulo`, `url`, `idioma`, `nivel`, `nota`, `empezar`

Rules for the sheet:

- `pelicula` must start with "Nueve reinas" or "NN".
- `nivel` is Fácil, Medio or Difícil.
- Put "sí" in `empezar` to mark a reading as **Para empezar**.
- Keep the column names in the first row as they are.

If the sheet can't be reached, the site shows the backup lists built into `index.html`. The links to the published sheet are near the bottom of `index.html` (`SHEET_BASE`).
