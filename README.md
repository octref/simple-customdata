# MOVED TO https://github.com/microsoft/vscode-custom-data

---

# Custom Data for HTML/CSS support in VS Code

This demonstrates Custom HTML/CSS data support for VS Code.

See https://code.visualstudio.com/updates/v1_31 for details.

## Usage

- Open this folder in VS Code 1.31+
- Try completion/hover in the test.html and test.css
- Edit data in html.json and css.json and reload to update the custom data

## Docs

- [HTML Custom Data](https://github.com/Microsoft/vscode-html-languageservice/blob/master/docs/customData.md)
- [CSS Custom Data](https://github.com/Microsoft/vscode-css-languageservice/blob/master/docs/customData.md)

## Settings

This setting checks the custom data against latest schema:

```json
{
  "json.schemas": [
    {
      "fileMatch": ["/html.json"],
      "url": "https://raw.githubusercontent.com/Microsoft/vscode-html-languageservice/master/docs/customData.schema.json"
    },
    {
      "fileMatch": ["/css.json"],
      "url": "https://raw.githubusercontent.com/Microsoft/vscode-css-languageservice/master/docs/customData.schema.json"
    }
  ]
}
```

## Related

See a real-world example at https://github.com/octref/svg-data.

## License

MIT
