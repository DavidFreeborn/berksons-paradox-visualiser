# Berkson's Paradox Visualiser

A lightweight interactive visualiser for showing how conditioning on a selection rule can induce a spurious negative association between two Gaussian variables.

## What it shows

This visualiser compares the population correlation with the correlation inside a selected sample. It is especially useful for illustrating Berkson's paradox under a rule such as:

- `aX + bY > T`

and the closely related near-fixed-total case:

- `|aX + bY - T| < δ`

It also notes that this is an instance of the explaining away effect.

## Files

- `index.html`: the complete visualiser, with no build step and no external dependencies.

## Quick deployment on GitHub Pages

1. Create a new GitHub repository.
2. Upload `index.html`.
3. Commit to the `main` branch.
4. In GitHub, go to `Settings` → `Pages`.
5. Under `Build and deployment`, choose `Deploy from a branch`.
6. Select the `main` branch and the `/ (root)` folder.
7. Save.
8. GitHub Pages will publish the visualiser at a URL of the form:
   `https://your-username.github.io/your-repo-name/`

## Embedding on another website

You can either:

1. host it as a standalone GitHub Pages page and link to it, or
2. embed it in an iframe, for example:

```html
<iframe
  src="https://your-username.github.io/your-repo-name/"
  width="100%"
  height="980"
  style="border:0; border-radius: 16px;"
  loading="lazy"
></iframe>
```

## Notes

- The visualiser always shows selected cases in blue and rejected cases in grey.
- The red line is fitted only within the selected sample.
- Press `Resample points` to see that the pattern is robust across different draws.
