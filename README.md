# Catbook
CATbook is a CATegory-centric Jekyll theme for bloggers. There is a switch button to toggle between dark mode and light mode. This theme is originally inspired from [Book](https://github.com/kkninjae/book).

[![LICENSE](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE) ![GENERATOR](https://img.shields.io/badge/made_with-jekyll-blue.svg) ![VERSION](https://img.shields.io/badge/current_version-1.0-green.svg)

**Demo:** https://starry99.github.io/catbook/

![SCREENSHOT](https://starry99.github.io/catbook/assets/img/lmode.jpg)
![SCREENSHOT](https://starry99.github.io/catbook/assets/img/dmode.jpg)

## Setup

```sh
$ git clone https://github.com/starry99/catbook
$ jekyll serve

# Now you can start customization!
```

## Make it yours

If you want to create a new category, you need to create `*name*.html` in the `categories` folder. And add the following content:
```html
---
layout: page
type: *name*
---

{% include archive.html %}
```
Then the number of pages in the category will be displayed.

## License

[MIT License](https://opensource.org/licenses/MIT)
