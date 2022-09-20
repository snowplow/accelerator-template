+++
title = "Deploy"
weight = 4
+++

To deploy the hugo site, add the attached `deploy.yml` and save it in a `workflows` folder. 

{{%attachments style="blue"/%}}

Edit the environment variables below to match your acclerator. Once you push to main the accelerator should be available on the gh-pages site.

```markdown
env:
    TITLE: YOUR_TITLE_HERE
    DESCRIPTION: YOUR_DESCRIPTION_HERE
    BASE_URL: https://docs.snowplow.io/GITHUB-REPO-NAME
    AUTHOR: AUTHOR
    LANDING_PAGE_URL: /GITHUB-REPO-NAME
```

