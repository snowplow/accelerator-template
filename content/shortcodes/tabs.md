+++
title = "Tabs"
weight = 3
+++

Tabs can be handy for providing code snippets for multiple languages or providing configuration in different formats.

```markdown
{{</* tabs groupId="tab_id" */>}}
{{%/* tab name="Tab 1" */%}}

### Tab 1

{{%/* /tab */%}}
{{%/* tab name="Tab 2" */%}}

### Tab 2

{{%/* /tab */%}}
{{</*/tabs */>}}
```

{{<tabs groupId="tab_id">}}
{{% tab name="Tab 1" %}}

### Tab 1

{{% /tab %}}
{{% tab name="Tab 2" %}}

### Tab 2

{{% /tab %}}
{{</tabs>}}

