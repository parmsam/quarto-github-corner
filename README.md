# Github Corner Extension For Quarto

This extension adds a GitHub corner to your Quarto document. A [GitHub corner](https://tholman.com/github-corners/) is a small SVG image that links to a URL of your choice. As the name suggests, it is typically used to link to a GitHub repository and placed in the top-right or top-left corner of a webpage.

## Installing


```bash
quarto add parmsam/quarto-github-corner
```

This will install the extension under the `_extensions` subdirectory.
If you're using version control, you will want to check in this directory.

## Using

To use the extension, add the following to your quarto (`.qmd`) file front matter:

```yaml
filters:
  - github-corner
```

Next, you can customize the corner by setting the following parameters in the front matter under `github-corner`.

- `url`: The URL to which the corner should link. This is a required parameter. Please ensure that you use the full URL, including the protocol (e.g., `https://www.github.com/parmsam/quarto-github-corner`).
- `logo-color`: The color of the logo. This can be any valid CSS color. The default is `#fff`.
- `background-color`: The color of the background. This can be any valid CSS color. The default is `#151513f`.
- `size`: The size of the corner in pixels. The default is `80`.
- `position`: The position of the corner. This can be either `left` or `right`. The default is `right`.

Here's the front matter I used in [example.qmd](example.qmd):

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

