# GoSF - CSS to Go Styling Functions Converter

Welcome to GoSF, a helper website designed to convert your CSS into Go styling functions for zui in web mode. zui is a Go library for building user interfaces, and you can learn more about it at [zui.dev](https://zui.dev).

## Features

- **CSS to Go Conversion**: Easily convert your CSS styles into Go functions compatible with zui/web.
- **User-Friendly Interface**: Simple and intuitive interface to streamline your workflow.
- **Instant Preview**: See the results of your conversions in real-time.

## Getting Started

1. **Visit the Website**: Go to [GoSF](https://zui.dev/gosf) to start converting your CSS.
2. **Input CSS**: Paste your CSS code into the input field.
3. **Generate Go Functions**: Click the convert button to generate Go styling functions.
4. **Copy and Use**: Copy the generated code and use it in your zui projects.

## Example

### CSS Input
```css
.button {
    background-color: #4CAF50;
    color: white;
    padding: 15px 32px;
    text-align: center;
    text-decoration: none;
    display: inline-block;
    font-size: 16px;
}
```

### Go Output
```go
func ButtonStyle(e *ui.Element) *ui.Element {
	e = doc.CSS.Container.Style.BackgroundColor.Value("#4CAF50")(e)
	e = doc.CSS.Container.Style.Color.White(e)
	e = doc.CSS.Container.Style.Padding.Value("15px 32px")(e)
	e = doc.CSS.Container.Style.TextAlign.Center(e)
	e = doc.CSS.Container.Style.TextDecoration.Value("none")(e)
	e = doc.CSS.Container.Style.Display.Value("inline-block")(e)
	e = doc.CSS.Container.Style.FontSize.Value("16px")(e)
	return e
}
```

## License

(GoSF is licensed under the MIT License unlike zui which is source available. See the [LICENSE](LICENSE) file for details.)

## Contact

For any questions or feedback, please reach out to us at [info@zui.dev](mailto:sinfo@zui.dev).

Happy Coding!
