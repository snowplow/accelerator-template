+++
title = "Creating Snowplow Accelerators"
menuTitle="Introduction"
chapter = false
weight = 1
post = ""

aliases = [
    "/en/",
    "/en/introduction/"
]
+++

#### Introduction

Welcome to the **Snowplow Accelerators** accelerator. Accelerators empower users to efficiently gain value from Snowplow’s technology. This guide covers how to make use of the accelerators template and some general style guidance.

#### Who is this guide for?
- Snowplow employees looking to get started with Accelerators

#### What you will learn
- Generate a hugo site
- What content to include/exclude

{{<mermaid>}}
gantt
        dateFormat  HH-mm
        axisFormat %M
        section 1. Upload
        1h          :upload, 00-00, 1m
        section 2. Model
        2h          :model, after upload, 2m
        section 3. Visualise
        3h          :visualise, after model, 3m
        section 4. Track
        4h          :track, after visualise, 4m
        section 5. Enrich
        1h          :enrich, after track, 1m
        section 6. Next steps
        2h          :next steps, after enrich, 2m

{{</mermaid >}}

***

#### Prerequisites

**Modeling and Visualisation**
- dbt CLI installed / dbt Cloud account available
  - New dbt project created and configured
- Python 3 Installed
- Snowflake account and a user with access to create schemas and tables

**Tracking and Enrichment**
- Snowplow pipeline
- Web app to implement tracking

{{% notice info %}}
Please note that Snowflake will be used for illustration but the snowplow-web dbt package also supports **BigQuery, Databricks, Postgres** and **Redshift**. Further adapter support for this accelerator coming soon!
{{% /notice %}}
