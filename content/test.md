---
views:
    kursrepo:
        region: sidebar-left
        template: anax/v2/block/default
        data:
            meta:
                type: single
                route: block/om-left-sidebar

    redovisa:
        region: sidebar-right
        template: anax/v2/block/default
        data:
            meta:
                type: single
                route: block/om-right-sidebar
---

Test
=========================

Testsida för Markdown

* Unordered list

1. Ordered list
  1. Ordered sub-list
  2. Ordered sub-list
2. Ordered list
  * Unordered sub-list
  * Unordered sub-list

# h1 header

### h3 header


*italic*

**strong**

[Inline style link](https://www.google.se)

[Inline style link with title](https://www.google.se "Google")

Images:

![Jester](image/jester.jpg?width=200)
