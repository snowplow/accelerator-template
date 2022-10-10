+++
title = "Deploy"
weight = 4
+++

To deploy the hugo site edit the `HUGO_BASEURL` in `netlify.toml` to the url for your site.

```toml
[build]
...
HUGO_BASEURL = 'https://docs.snowplow.io/accelerators/{{YOUR BASE URL}}/'
BUILD_OUTPUT_PATH = '/accelerators/{{YOUR BASE URL}}/'
...

[[redirects]]
...
to = "/accelerators/{{YOUR BASE URL}}/:splat"
...
```

You will also need to update the information in the `config.toml`.

```toml
title = "{{ACCELERATOR TITLE}}"
baseURL = "https://docs.snowplow.io/accelerators/{{YOUR BASE URL}}/"

[params]
  description = "{{ACCELERATOR DESCRIPTION}}"
  author = "{{AUTHOR NAMES}}"
```

Upon PR, a deployment preview will be available to check you are happy with the build as below. Changes will be visible as you commit so there is no need to create multiple PRs.

![deploy](../images/deploy_preview.png)


