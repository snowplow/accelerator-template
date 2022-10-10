+++
title = "Folder Structure"
weight = 1
+++

Hugo is website generator used to build accelerators. This allows us to quickly generate a site, with custom theming and integration with Github pages.

Most of the Hugo code sits in the [accelerator-web-ui-template](https://github.com/snowplow-incubator/accelerator-web-ui-template) repo, but for the site to get generated a few things are needed.

- **Content:** This folder contains all of the markdown files that make up the content of the site
- **Scripts:** This folder contains the build script to deploy the site
- **Config Files:** Additional config files to define the site parameters

An example of the folder structure can be found in the download below:

{{%attachments style="blue"/%}}

#### Content Folder
The content folder defines the structure of the site. Each folder makes up a chapter which then generates a side-navbar, for example:

{{% notice info %}}
The `Introduction` page goes in the Content folder as `_index.md` and any images on that page should go in an `images` folder within `content`.
{{% /notice %}}

![content](../images/content.png?width=50pc)


#### Chapters
For every chapter, an `_index.md` file is required. This is the entry point for the chapter and also contains metadata such as the title and position the chapter takes. This is specified at the top of the page, the metadata for the Hugo Chapter page is as below:

```markdown
+++
title="Hugo"
chapter = true
weight = 2
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

