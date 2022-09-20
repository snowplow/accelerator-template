+++
title = "Attachments"
weight = 4
+++

The Attachments shortcode displays a list of files attached to a page. This is useful for providing sample data and notebooks.

The attachments need to be placed in a `pages.files` folder. For example, if a page is named `test_page` attachments need to be added to a folder called `test_page.files`.

```
{{%/*attachments style="blue"/*/%}}
```

renders to

{{%attachments style="blue"/%}}
