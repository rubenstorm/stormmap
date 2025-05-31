# StormMap — Hugo Sitemap Shortcode by Ruben Storm

**StormMap** is a minimalist, colorful, and flexible shortcode for Hugo that renders a structured sitemap or archive view of your content. It supports nested sections, icons, and multiple designs.

---

## 🚀 Features

- Minimal, semantic HTML output
- Multiple visual designs: `minimal`, `color`, `nostr`, `green`, `red`, `blue`, `orange`
- Nested sections and pages
- Optional branded footer (Storm logo or text)
- Inline icon support via Hugo partials
- Lightweight and theme-agnostic

---

## 📦 Installation

### Hugo Module (Recommended)

```bash
hugo mod get github.com/rubenstorm/stormmap
```

Add to your `config.toml`:

```toml
[module]
  [[module.imports]]
    path = "github.com/rubenstorm/stormmap"
```

**or**

Add to your `config.yaml`:

```toml
module:
  module.imports:
    path: "github.com/rubenstorm/stormmap"
```

---

## 🧩 Usage

Basic usage in content or templates:

```go-html-template
{{< stormmap >}}
```

### Optional Parameters

| Param      | Type   | Default   | Description                                      |
|------------|--------|-----------|--------------------------------------------------|
| `design`   | string | `minimal` | Visual style: see available options below        |
| `branding` | string | `true`    | Show StormMap branding (`true` or `false`)       |

### Examples

Colorful layout without branding:

```go-html-template
{{< stormmap design="color" branding="false" >}}
```

Nostr-style layout with icons and branding:

```go-html-template
{{< stormmap design="nostr" >}}
```

---

## 🎨 Design Options

| Value      | Description                            |
|------------|----------------------------------------|
| `minimal`  | Clean text-based layout with bullets    |
| `color`    | Sections and pages styled with colors   |
| `nostr`    | Nostr-inspired lightning icon layout    |
| `green`    | Green color variant                     |
| `red`      | Red color variant                       |
| `blue`     | Blue color variant                      |
| `orange`   | Orange color variant                    |

---

## 🚫 Hiding Pages

To hide specific pages or sections from StormMap, add this to their front matter:

### toml

```toml
hideStormMap = true
```

### yaml

```yaml
hideStormMap: true
```

---

## 📄 License

MIT License  
Copyright © Ruben Storm

---

## ⚡️ Support This Project

If you enjoy using StormMap, consider donating:

⚡️ [Donate Lightning](https://coinos.io/rubenstorm)


---

> Made with ♥ by [Ruben Storm](https://rubenstorm.github.io/)
