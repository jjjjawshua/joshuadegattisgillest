# joshua degattis-gillest — portfolio

Static site. No build step, no dependencies. Open `index.html` in a browser.

## Editing in VS Code

- **Add photos:** drop files into `images/`, then add a line to the `WORKS` array at the bottom of `index.html`:
  ```js
  { src: 'images/my-photo.jpeg', title: 'title here', year: '2026', ratio: '3/2' },
  ```
  `ratio` is the crop shown in the grid — `3/2` landscape, `3/4` portrait, `1/1` square.
- **Hero image:** replace `images/hero.jpeg` (or change the `src` in the `#home` section).
- **Copy:** about / contact text lives directly in the HTML.
- **Colors & type:** the `:root` variables at the top of the `<style>` block.

## Publishing with GitHub Pages

1. Create a repo and push this folder's contents.
2. Repo → Settings → Pages → Source: `main`, folder `/ (root)`.
3. Live at `https://<user>.github.io/<repo>/`.

Local preview: `python3 -m http.server` then open `localhost:8000`.
