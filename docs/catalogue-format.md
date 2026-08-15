# Community template catalogue

`catalogue.json` is the versioned entry point for templates that can be offered by HTML Advanced.

```json
{
  "version": 1,
  "templates": [
    {
      "id": "example-template",
      "title": "Example template",
      "description": "A short description.",
      "language": "en",
      "liquid": false,
      "version": "1",
      "source": "templates/example-template.html"
    }
  ]
}
```

Each template must have a stable lowercase identifier, an HTML source beneath `templates/`, a language, a version, and an explicit `liquid` flag. The module validates the entire manifest before it caches it. A manifest without templates is valid and lets installations safely prepare for future community templates.
