+++
title = "Folder Structure"
weight = 1
+++

#### Hugo Site Generation
Hugo is website generator used to build accelerators. This allows us to quickly generate a site, with custom theming and integration with Github pages.

Most of the Hugo code sits in the [accelerator-web-ui-template](https://github.com/snowplow-incubator/accelerator-web-ui-template) repo, but for the site to get generated a few things are needed.

- **Content:** This folder contains all of the markdown files that make up the content of the site
- **Workflows:** This folder contains the github action with site specific configuration

#### Content Folder
The content folder defines the structure of the site. Each folder makes up a chapter which then generates a navbar as below:

![content](../images/content.png)


#### Chapters
For every chapter, an `_index.md` file is required. This is the entry point for the chapter and also contains metadata such as the title and position the chapter takes. This is specified at the top of the page, the metadata for the Hugo Chapter page is as below:

{{% notice note %}}
The metadata section doesn't support comments so these need to be deleted
{{% /notice %}}

```markdown
+++
title="Hugo"
chapter = true
weight = 2
pre = ""
post = ""
+++
```

A short description of the chapter can then be added in markdown.

#### Content
The content is also stored in markdown files within the content folder and can be named anything.

These pages also have metadata stored in them defining the page title and order they're to be displayed in. For example this page has the markdown below.

```markdown
+++
title = "Setup"
weight = 1
+++
```

