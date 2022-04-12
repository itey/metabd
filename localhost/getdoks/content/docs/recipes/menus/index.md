---
title: "Menus"
description: "Add pages or links to the main, social, docs, or footer menu. Set page level navigation."
lead: "Add pages or links to the main, social, docs, or footer menu. Set page level navigation."
date: 2020-11-23T11:55:36+01:00
lastmod: 2020-11-23T11:55:36+01:00
draft: false
images: []
menu:
  docs:
    parent: "recipes"
weight: 150
toc: true
---

{{< img-simple src="navigation-mobile.png" alt="Navigation Mobile" class="d-block mx-auto shadow my-5" >}}
{{< img-simple src="navigation-structure-mobile.png" alt="Navigation Structure Mobile" class="d-block mx-auto my-5 shadow" >}}

See also the Hugo docs: [Menus](https://gohugo.io/content-management/menus/).

```bash
./config/_default/menus/menus.en.toml
```

## Global navigation

### Add to main menu

```toml
[[main]]
  name = "Docs"
  url = "/docs/prologue/introduction/"
# url = "/docs/1.0/prologue/introduction/"
  weight = 10

[[main]]
  name = "Blog"
  url = "/blog/"
  weight = 20

[[main]]
  name = "Get Started"
  weight = 30
  identifier = "get-started"
  url = "/docs/prologue/introduction/"

[[main]]
  name = "Quick Start"
  weight = 40
  identifier = "quick-start"
  url = "/docs/prologue/quick-start/"
  parent = "get-started"

[[main]]
  name = "Tutorial"
  weight = 50
  identifier = "tutorial"
  url = "https://getdoks.org/tutorial/introduction/"
  parent = "get-started"
```

### Add to social menu

{{< alert icon="👉" text="Doks uses <a href=\"https://feathericons.com/\">Feather Icons</a>" />}}

```toml
[[social]]
  name = "Twitter"
  pre = "<svg xmlns=\"http://www.w3.org/2000/svg\" width=\"20\" height=\"20\" viewBox=\"0 0 24 24\" fill=\"none\" stroke=\"currentColor\" stroke-width=\"2\" stroke-linecap=\"round\" stroke-linejoin=\"round\" class=\"feather feather-twitter\"><path d=\"M23 3a10.9 10.9 0 0 1-3.14 1.53 4.48 4.48 0 0 0-7.86 3v1A10.66 10.66 0 0 1 3 4s-4 9 5 13a11.64 11.64 0 0 1-7 2c9 5 20 0 20-11.5a4.5 4.5 0 0 0-.08-.83A7.72 7.72 0 0 0 23 3z\"></path></svg>"
  url = "https://twitter.com/gethyas"
  weight = 10

[[social]]
  name = "GitHub"
  pre = "<svg xmlns=\"http://www.w3.org/2000/svg\" width=\"20\" height=\"20\" viewBox=\"0 0 24 24\" fill=\"none\" stroke=\"currentColor\" stroke-width=\"2\" stroke-linecap=\"round\" stroke-linejoin=\"round\" class=\"feather feather-github\"><path d=\"M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22\"></path></svg>"
  url = "https://github.com/h-enk/doks"
  post = "v0.1.0"
  weight = 20
```

## Section navigation

### Configure

In `./config/_default/params.toml` set menu options:

```toml
[menu]
  [menu.section]
    auto = true
    collapsibleSidebar = true
```

You now have the option to let Doks __auto__ generate the section menu from the directory folder (tree) structure. No manual configuration needed and respects set weight. Available for both the collapsibile section menu and the default one.

### Add to docs menu

Set __first__ level menu items in `./config/_default/menus/menus.en.toml`:

```toml
..
[[docs]]
  name = "Prologue"
  weight = 10
  identifier = "prologue"
  url = "/docs/prologue/"

[[docs]]
  name = "Help"
  weight = 60
  identifier = "help"
  url = "/docs/help/"

# [[docs]]
#   name = "Lorem"
#   weight = 70
#   identifier = "lorem"
#   url = "/docs/lorem/"
..
```

Set __second__ level menu items in the frontmatter of a docs page (manual mode):

```md
..
menu:
  docs:
    parent: "lorem"
    identifier: "ipsum"
..
```

Set __third__ level menu items in the frontmatter of a docs page (manual mode):

```md
..
menu:
  docs:
    parent: "ipsum"
..
```

## Page navigation

### Set levels

The On this page (Table of Contents) section is automatically generated. In `./config/_default/markup.toml`, set the levels you'd like to show:

```toml
[tableOfContents]
  endLevel = 3
  ordered = false
  startLevel = 2
```

## Footer navigation

### Add to footer menu

```toml
[[footer]]
  name = "Privacy"
  url = "/privacy-policy/"
  weight = 10
```
