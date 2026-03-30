# fontfyi

[![crates.io](https://img.shields.io/crates/v/fontfyi.svg)](https://crates.io/crates/fontfyi)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

Google Fonts metadata, CSS generation, and font pairing — API client for [fontfyi.com](https://fontfyi.com).

> **Try the interactive tools at [fontfyi.com](https://fontfyi.com)**

## Install

`cargo add fontfyi`

## Quick Start

```rust
use fontfyi::Client;

#[tokio::main]
async fn main() -> Result<(), Box<dyn std::error::Error>> {
    let client = Client::new();
    let result = client.search("inter").await?;
    println!("{} results", result.total);
    Ok(())
}
```

## Also Available

| Platform | Package | Link |
|----------|---------|------|
| **Python** | `pip install fontfyi` | [PyPI](https://pypi.org/project/fontfyi/) |
| **npm** | `npm install fontfyi` | [npm](https://www.npmjs.com/package/fontfyi) |
| **Go** | `go get github.com/fyipedia/fontfyi-go` | [pkg.go.dev](https://pkg.go.dev/github.com/fyipedia/fontfyi-go) |
| **Rust** | `cargo add fontfyi` | [crates.io](https://crates.io/crates/fontfyi) |
| **Ruby** | `gem install fontfyi` | [rubygems](https://rubygems.org/gems/fontfyi) |

## Embed Widget

Embed [FontFYI](https://fontfyi.com) widgets on any website with [fontfyi-embed](https://widget.fontfyi.com):

```html
<script src="https://cdn.jsdelivr.net/npm/fontfyi-embed@1/dist/embed.min.js"></script>
<div data-fontfyi="entity" data-slug="inter"></div>
```

Zero dependencies · Shadow DOM · 4 themes (light/dark/sepia/auto) · [Widget docs](https://widget.fontfyi.com)

## Links

- [FontFYI](https://fontfyi.com) — Main site
- [API Documentation](https://fontfyi.com/developers/)
- [OpenAPI Spec](https://fontfyi.com/api/openapi.json)
- [Glossary](https://fontfyi.com/glossary/)

## License

MIT
