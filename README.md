# Github Corner Extension For Quarto

This extension adds a GitHub corner to your Quarto book. The GitHub corner is a small SVG image that links to a URL of your choice.

## Installing


```bash
quarto add parmsam/github-corner
```

This will install the extension under the `_extensions` subdirectory.
If you're using version control, you will want to check in this directory.

## Using

To use the extension, add the following to your `_quarto.yml` file:

```yaml
filters:
  - github-corner
```

Next, you can customize the corner by setting the following parameters in the front matter under `github-corner`.

- `url`: The URL to which the corner should link. This is a required parameter. Please ensure that you use the full URL, including the protocol (e.g., `https://www.github.com/parmsam/`).
- `logo-color`: The color of the logo. This can be any valid CSS color. The default is `#fff`.
- `background-color`: The color of the background. This can be any valid CSS color. The default is `#151513f`.
- `size`: The size of the corner in pixels. The default is `80`.
- `position`: The position of the corner. This can be either `left` or `right`. The default is `right`.

Here's the front matter I used in (example.qmd)[example.qmd]:

```yaml
filters:
  - github-corner
github-corner:
  url: "https://www.github.com/parmsam/quarto-github-corner"
  logo-color: "white"
  background-color: "#1c84e5"
  size: 150
  position: "left"
```

## Example

Here is the source code for a minimal example: [example.qmd](example.qmd).

