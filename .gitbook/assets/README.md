# GitBook assets

Drop images here to reference them from any wiki page.

## Expected files

| File | Used on | Purpose |
|---|---|---|
| `logo.png` | `README.md` | Wiki logo shown at the top of the intro page |
| `banner.png` | `README.md` (cover) | Hero banner displayed as the cover image |

## How to add a new image

1. Save the image inside this folder (`.gitbook/assets/`)
2. Use standard markdown image syntax wherever you want to embed it:

   ```markdown
   ![Alt text](../.gitbook/assets/my-image.png)
   ```

   The relative path depends on where the markdown file lives. For example, from `classes/vampire.md` you'd write `../.gitbook/assets/vampire.png`.

3. For the **cover image** on any page, set it in the page front-matter:

   ```yaml
   ---
   cover: .gitbook/assets/banner.png
   coverY: 0
   ---
   ```

## Conventions

- Prefer `.png` for logos/banners, `.webp` or `.jpg` for screenshots
- Keep filenames lowercase, hyphenated (`chief-telamon.png`, not `Chief Telamon.PNG`)
- Under **1 MB per image** when possible — GitBook mirrors everything through its CDN
- Group related images with a prefix: `boss-pluto.png`, `boss-leviathan.png`, `biome-gelo.png`
